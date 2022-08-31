# Test-driven development

A style of programming in which three activities are tightly interwoven: Coding, testing (in the form of unit testing), and design (in the form of refactoring). The whole process can be described as follows:

- write a single 'unit test' which describes an aspect of the program.
- run the tests which should result in failed test cases because the program lacks that feature.
- write just "enough code" the simplest possible to make the test pass.
- refactor the code to make it conform to the criteria.
- repeat accumulating unit tests and features over time.