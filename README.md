# kotlin-TDD-Exersize-III

```
import org.assertj.core.api.Assertions
import java.lang.reflect.Array
import kotlin.test.Test
//import com.kotlination.splitstring


class wrapperTests{
//    @Test
//    fun assertionWrapReturnsString(){
//        //Arrange
//        //stub / mock
//        val wrapper : Wrapper = Wrapper()
//Act
//        //do something with the method under test
//        var text = "text"
//        val wrap = wrapper.wrap(text)
// Assert
// assert…. test.. test..
//        Assertions.assertThat(wrap).isEqualTo(text)
//    }
    @Test

    fun assertionWrapReturnsText(){
        //Arrange
        //stub mock
        val wrapper : Wrapper = Wrapper()
// Act
//do something with the method under test
        var str = "text"
        var kolnr = 1

        val wrap = wrapper.wrap(str, kolnr)
// Assert
//assert…. test.. test..
        Assertions.assertThat(wrap).isEqualTo("t\ne\nx\nt")
    }
 
    @Test
    fun assertionWrapReturnsHello(){
//Arrange
//stub / mock
        val wrapper : Wrapper = Wrapper()
// Act
//do something with the method under test
        var str = "line"
        var kolnr = 1

        val wrap = wrapper.wrap(str, kolnr)
// Assert
  //assert…. test.. test..
        Assertions.assertThat(wrap).isEqualTo("l\ni\nn\ne")
    }


}

class Wrapper{
    fun wrap(x : String, y : Int) : String{
        var splitString = x.toCharArray()
        var outcome = splitString.forEach {
            println(it)
        }
return outcome
    }
}
```
