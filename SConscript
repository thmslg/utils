Import('env')

sources = [
'Sources/ListenerSubject.cpp',
] 
library = env.Library('utils', sources )

testList =  [
'UnitTest/DelegateBooleanParameter.t.h',
'UnitTest/ObserverSubject.t.h',
]

env.Append(LIBS=library)
env.CxxTest('testrunner',testList, CXXFLAGS='-Wall -W -Wextra')

Return('library')