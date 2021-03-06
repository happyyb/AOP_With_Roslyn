# AOP_With_Roslyn

[![GitHub license](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/ignatandrei/Interpreter/blob/master/LICENSE)  

[![NuGet](https://img.shields.io/nuget/v/dotnet-aop.svg)](https://www.nuget.org/packages/dotnet-aop)

[![Build status](https://ci.appveyor.com/api/projects/status/q63slvkomrifq3ha?svg=true)](https://ci.appveyor.com/project/ignatandrei/aop-with-roslyn)


[![codecov](https://codecov.io/gh/ignatandrei/AOP_With_Roslyn/branch/master/graph/badge.svg)](https://codecov.io/gh/ignatandrei/AOP_With_Roslyn)


 
 
 
Install as global tool as

dotnet tool install -g dotnet-aop

go to your solution folder
run

dotnet aop


For customizing what you want to insert at every method at first line and last line, see https://github.com/ignatandrei/AOP_With_Roslyn/blob/master/AOPRoslyn/processme.txt


You can save the document in your solution root and execute with


dotnet aop &lt;your file name&gt;



The following table is generated by gathering statistics from dotnet aop tests with dotnet aop integrated :



| Class             | Method(Line)                                | NumberHit | TotalTime | AverageTime |
|-------------------|---------------------------------------------|-----------|-----------|-------------|
| TestLineDirective | TestException(55)                           | 1         | 2881      | 2881        |
| TestArguments     | TestArgumentsFor(13)                        | 1         | 543       | 543         |
| RewriteCodeFile   | Rewrite(44)                                 | 5         | 533       | 106         |
| TestLineDirective | TestNoLineRefactoring(125)                  | 1         | 79        | 79          |
| RewriteCode       | RewriteCodeMethod(45)                       | 13        | 566       | 43          |
| TestSerialize     | TestSerializeRewriteCodeFolder(14)          | 1         | 26        | 26          |
| TestComment       | TestUnComment(12)                           | 1         | 22        | 22          |
| TestCommandLine   | TestMethodRewriterSimple(9)                 | 1         | 15        | 15          |
| TestRewriteCode   | TestAOPFolder(78)                           | 1         | 11        | 11          |
| RewriteCodeFolder | Rewrite(69)                                 | 1         | 9         | 9           |
| MethodRewriter    | VisitMethodDeclaration(72)                  | 23        | 140       | 6           |
| TestRegion        | TestOneRegion(11)                           | 1         | 5         | 5           |
| TestAOPExtension  | TestExtensionIsModifierOnEnum(12)           | 1         | 5         | 5           |
| TestInitializeAll | Init(14)                                    | 1         | 4         | 4           |
| RewriteAction     | UnSerializeMe(52)                           | 3         | 14        | 4           |
| RewriteAction     | SerializeMe(33)                             | 3         | 12        | 4           |
| TestRewriteCode   | TestAOPFile(64)                             | 1         | 3         | 3           |
| TestSerialize     | TestSerializeRewriteCodeFile(26)            | 1         | 1         | 1           |
| TestRewriteCode   | TestModifierMethodNoCodeInFile(13)          | 1         | 1         | 1           |
| TestLineDirective | TestLineSimple(18)                          | 1         | 0         | 0           |
| TestLastLine      | TestMethodRewriterLastLine(9)               | 1         | 0         | 0           |
| TestCommandLine   | TestMethodRewriterAddVariable(47)           | 1         | 0         | 0           |
| Extensions        | IsOnEnum(78)                                | 40        | 0         | 0           |
| TestSerialize     | TestSerializeRewriteCodeFolderFormatter(42) | 1         | 0         | 0           |
| TestRewriteCode   | TestModifierMethod(25)                      | 1         | 0         | 0           |

