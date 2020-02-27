genrule(
  name = "test", 
  out = "out.txt",
  cmd = "echo $(classpath :foo) > ${OUT}"
)

java_library(
  name = "foo",
  srcs = ["Foo.java"],
  deps = [":bar"]
)

java_library (
  name = "bar",
  srcs = ["Bar.java"],
  deps = [":baz"]
)

java_library (
  name = "baz",
  srcs = ["Baz.java"]
)
