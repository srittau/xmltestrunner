This is a test runner for the unittest module, Python's version of the xUnit
framework. The test runner captures the test results in a XML file that is
compatible with the XML output of JUnit. Various tools, like continuous
integration servers can parse this output.

Sample usage:

```python
import unittest

from xmlrunner import XMLTestRunner

loader = unittest.TestLoader()
tests = loader.discover()
runner = XMLTestRunner()
runner.run(tests)
```
