# 0.2.4

* Standardized Errors with TelepatError object
* Implemented Delta.formPatches to more easily form patches from objects
* Moved messaging client from telepat-worker to telepat-models to be reusable by other components
* Added 'type' field to application, context and admin objects

# 0.2.3

* Replaced couchbase with elasticsearch through adapters
* Fixed many bugs
* Added email field to Deltas (used by user operations)
* Admin create throws 409 error when admin with that email address already exists
* Implemented admin.delete
* getDevices returns the corect error message when missing
* Implemented Delta.processObject which can be used by all update operations

# 0.2.2

* Release full of bug fixes

# 0.2.1

* Important performance issue fixed: all Models operations require context id when getting the object from database

# 0.2.0

* Implemented Channel and Delta classes to further separate code logic
* Added password field to user objects
* Fixed subscribe.remove and .add
* Fixed application schema keys
* Fixed device persistent udid key
* Return 404 error when unsubscribing with an invalid subscription

# 0.1.2

* Added LICENSE and README files
* get All Models and get All Contexts now return an array in the callback instead of hash map

# 0.1.0

* Initial Release