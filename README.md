You're at the zoo... all the meerkats look weird. Something has gone terribly wrong - someone has gone and switched their heads and tails around!

Save the animals by switching them back. You will be given an array which will have three values (tail, body, head). It is your job to re-arrange the array so that the animal is the right way round (head, body, tail).

Same goes for all the other arrays/lists that you will get in the tests: you have to change the element positions with the same exact logics

Simples!



This are the tests:

###
import org.junit.Test;
import static org.junit.Assert.assertArrayEquals;
import org.junit.runners.JUnit4;

public class SolutionTest {
    @Test
    public void exampleTest1() {
        assertArrayEquals(new String[]{ "head", "body", "tail" },
          WrongEndHead.fixTheMeerkat(new String[]{ "tail", "body", "head" }));
    }
    
    @Test
    public void exampleTest2() {
        assertArrayEquals(new String[]{ "heads", "body", "tails" },
          WrongEndHead.fixTheMeerkat(new String[]{ "tails", "body", "heads" }));
    }
    
  
    @Test
    public void exampleTest3() {
        assertArrayEquals(new String[]{ "top", "middle", "bottom" },
          WrongEndHead.fixTheMeerkat(new String[]{ "bottom", "middle", "top" }));
    }
    
    @Test
    public void exampleTest4() {
        assertArrayEquals(new String[]{ "upper legs", "torso", "lower legs" },
          WrongEndHead.fixTheMeerkat(new String[]{ "lower legs", "torso", "upper legs" }));
    }
    
    @Test
    public void exampleTest5() {
        assertArrayEquals(new String[]{ "sky", "rainbow", "ground" },
          WrongEndHead.fixTheMeerkat(new String[]{ "ground", "rainbow", "sky" }));
    }
}
