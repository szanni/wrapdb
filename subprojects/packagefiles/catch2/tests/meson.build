# define the sources of the self test
# Please keep these ordered alphabetically
self_test_sources = [
  'SelfTest/TestRegistrations.cpp',
  'SelfTest/IntrospectiveTests/Clara.tests.cpp',
  'SelfTest/IntrospectiveTests/CmdLine.tests.cpp',
  'SelfTest/IntrospectiveTests/CmdLineHelpers.tests.cpp',
  'SelfTest/IntrospectiveTests/ColourImpl.tests.cpp',
  'SelfTest/IntrospectiveTests/Details.tests.cpp',
  'SelfTest/IntrospectiveTests/FloatingPoint.tests.cpp',
  'SelfTest/IntrospectiveTests/GeneratorsImpl.tests.cpp',
  'SelfTest/IntrospectiveTests/InternalBenchmark.tests.cpp',
  'SelfTest/IntrospectiveTests/PartTracker.tests.cpp',
  'SelfTest/IntrospectiveTests/RandomNumberGeneration.tests.cpp',
  'SelfTest/IntrospectiveTests/Reporters.tests.cpp',
  'SelfTest/IntrospectiveTests/Tag.tests.cpp',
  'SelfTest/IntrospectiveTests/TestCaseInfoHasher.tests.cpp',
  'SelfTest/IntrospectiveTests/TestSpecParser.tests.cpp',
  'SelfTest/IntrospectiveTests/TextFlow.tests.cpp',
  'SelfTest/IntrospectiveTests/Sharding.tests.cpp',
  'SelfTest/IntrospectiveTests/Stream.tests.cpp',
  'SelfTest/IntrospectiveTests/String.tests.cpp',
  'SelfTest/IntrospectiveTests/StringManip.tests.cpp',
  'SelfTest/IntrospectiveTests/Xml.tests.cpp',
  'SelfTest/IntrospectiveTests/ToString.tests.cpp',
  'SelfTest/IntrospectiveTests/UniquePtr.tests.cpp',
  'SelfTest/TimingTests/Sleep.tests.cpp',
  'SelfTest/UsageTests/Approx.tests.cpp',
  'SelfTest/UsageTests/BDD.tests.cpp',
  'SelfTest/UsageTests/Benchmark.tests.cpp',
  'SelfTest/UsageTests/Class.tests.cpp',
  'SelfTest/UsageTests/Compilation.tests.cpp',
  'SelfTest/UsageTests/Condition.tests.cpp',
  'SelfTest/UsageTests/Decomposition.tests.cpp',
  'SelfTest/UsageTests/EnumToString.tests.cpp',
  'SelfTest/UsageTests/Exception.tests.cpp',
  'SelfTest/UsageTests/Generators.tests.cpp',
  'SelfTest/UsageTests/Message.tests.cpp',
  'SelfTest/UsageTests/Misc.tests.cpp',
  'SelfTest/UsageTests/ToStringByte.tests.cpp',
  'SelfTest/UsageTests/ToStringChrono.tests.cpp',
  'SelfTest/UsageTests/ToStringGeneral.tests.cpp',
  'SelfTest/UsageTests/ToStringOptional.tests.cpp',
  'SelfTest/UsageTests/ToStringPair.tests.cpp',
  'SelfTest/UsageTests/ToStringTuple.tests.cpp',
  'SelfTest/UsageTests/ToStringVariant.tests.cpp',
  'SelfTest/UsageTests/ToStringVector.tests.cpp',
  'SelfTest/UsageTests/ToStringWhich.tests.cpp',
  'SelfTest/UsageTests/Tricky.tests.cpp',
  'SelfTest/UsageTests/VariadicMacros.tests.cpp',
  'SelfTest/UsageTests/MatchersRanges.tests.cpp',
  'SelfTest/UsageTests/Matchers.tests.cpp'
]

# This isn't as good as the CMake tests, but it proves that we've
# actually put something in the library files.
self_test = executable(
  'self_test',
  self_test_sources,
  include_directories : '../src',
  link_with : [ catch2_with_main, catch2 ]
)

test('SelfTest', self_test)
