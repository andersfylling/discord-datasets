# discord-datasets
datasets for Discord library developers to ensure their cache implementation is working.

It is important to start with a empty cache and remember that the json files here represents the "d" content of fresh websocket events.

In the events dir you will find a directory representing a event type. These contains two types of files, the numerated ones which are actual events and the "state.json" file which is what your cache is expected to look like after you have handled all the events.

> Note! that the state.json does not store default values. eg. false, 0, "", [], etc. This is to save space when the json file contains millions of objects.

### Formatting
User data is expected to be in their own cache repository. Meaning the state.json for all user related data will be a single array.