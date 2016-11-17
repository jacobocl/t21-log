# T21Log

Commons classes added to this library:
* T21Log

## How to add to your project
Pending

## How to use

### Setting up

In your application class or your launcher activity (or main/base activity) you should call these methods:

* T21Log.setLogTag(String) to set the tag of your application. This tag will be in the whole app.

* T21Log.setLogEnabled(boolean) to set enabled or disabled the log. If you don't call this method then nothing will be printed. Is a good practice call like this 'T21Log
    .setLogEnabled(BuildConfig.DEBUG);', in order to avoid print log messages in release versions.
    
### Printing logs

Some examples If you set your tag "[SAMPLE_APP]":

* `T21Log.d("Hello")`; --> 'D/[SAMPLE_APP]: Hello'

* `T21Log.d(CLASS_TAG, "Hello")`; --> 'D/[SAMPLE_APP]: [MainActivity] Hello' (if CLASS_TAG == '[MainActivity]')

* `T21Log.d(CLASS_TAG, "onCreate", "adding messages", 3, true, "separated by commas");` --> 'D/[SAMPLE_APP]: [MainActivity] onCreate adding messages 3 true separated by commas' (if CLASS_TAG == '[MainActivity]')

## Contributing to the project

Feel free to report any issues or suggest new features.

## License

Copyright 2016 Worldline Iberia

Licensed under the Apache License, Version 2.0 (the "License"); you may not use this file except in compliance with the License. You may obtain a copy of the License at

http://www.apache.org/licenses/LICENSE-2.0
Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the specific language governing permissions and limitations under the License.

