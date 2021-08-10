# Why Use Test Driven Development

## What is TDD?

_Test Driven Development (TDD) is a software development practice enabling developers to create proper specifications about how their code should be written and implemented. Fundamentally, TDD is a practice when a programmer writes a functional test before building a code._

_The idea of TDD originated in the middle of the 20th century, and since then has been applied in many areas. TDD was afterward rediscovered in 2002 by Kent Beck, an American Software Engineer and the creator of Extreme Programming methodology. He described it in his book Test Driven Development: By Example._

_The original description of TDD was in an ancient book about programming. It said you take the input tape, manually type in the output tape you expect, then program until the actual output tape matches the expected output. After I'd written the first xUnit framework in Smalltalk I remembered reading this and tried it out. That was the origin of TDD for me. When describing TDD to older programmers, I often hear, "Of course. How else could you program?" Therefore I refer to my role as "rediscovering" TDD. - Kent Beck_

The image below shows a typical test driven development cycle.

![TDD](https://codica-images-production.s3.eu-central-1.amazonaws.com/0c6dbb1613ad4f93b9c793a96a71efd8.webp)

This process includes the following stages:

    1- Writing a test that fails because of code absence (red).
    2- Writing a code after which the test is passed (green).
    3-Refactoring - checking the code structure and its improvement
       without changing its external behavior. The expected result of
       refactoring is obtaining a perfectly written code

By repeating this process for every single piece of functionality, a developer obtains full test code coverage, which will provide excellent design and easy application maintenance in the future.
***


# What are the advantages of TDD approach?

1. Better program design and higher code quality

        When writing tests, programmers first have to define a goal they will achieve with the code piece. Developers estimate an experience it will give and the way it will match with other pieces of the entire code. A developer keeps in mind everything, from an interface to a work plan.

        Besides, TDD strongly evolves with the DRY principle. It says programmers should avoid repeating code in different system parts. The principle invites developers to use small classes and functions for particular requirements. This helps clearly define the system objects and keep the codebase successive.

2. Detailed project documentation

        When writing tests for particular requirements, programmers immediately create a strict and detailed specification. It already includes all the likely users’ actions.

3. TDD reduces the time required for project development

        It’s widely known that both web and cross-platform apps like PWAs created with Test Driven Development take longer than ones created without TDD. Some sources mention the difference of about 30 percent.

        You would probably make a conclusion that TDD postpones your project delivery date. But is it really so?

        According to the study held by Eric Elliott, founder of Parallel Drive, maintenance of an application made without Test Driven Development implementation may take twice as much time as of an application created with TDD.

    ![](https://codica-images-production.s3.eu-central-1.amazonaws.com/2a39a5f3af33451593460e76bc648f1b.webp)


4. Code flexibility and easier maintenance

        When writing code, developers strive to get fewer bugs, which 
        considerably influences business spending.

5. With TDD you will get a reliable solution

        With TDD, both you and the developers can be sure about the
        reliability of the developed solution. That is, tests help to
        understand if everything goes right after refactoring or adding a
        new feature.

6. Save project costs in the long run

        And last but not least - with TDD implementation, the cost of project development will significantly decrease.

        This is the result of all the advantages mentioned previously, namely the following:

        1- The code that you will get will be maintainable, flexible and easy to extend.
        2- The solution will be reliable for any further enhancements or development.
        3- You will have ready documentation that can be used further on for any purposes.
        4- The quality of the product developed with TDD is significantly higher.