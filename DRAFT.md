## Structs (DTO)
PORO, Hashie, Struct, OpenStruct, Virtus, Hamster

## Principles
- DDD
- CQRS
- GRASP
- SOLID

# api
# cells
Encapsulate parts of your page into separate widgets. Mostly, used in views to replace a helper/partial mess.
# controllers
Everything related to parsing requests, sessions, protection, rendering templates, redirecting, flash messages.
# decorators
Allows functionality to be divided between classes with unique areas of concern.
Behavior could be added to an individual object, without affecting the original object.
For example you can wrap your models to extract presentation related logic from helpers.
# dto
Represents data as definite structures that carries data between processes.
Does not have any behavior, manipulates data only via accessors and mutators.
# entities
# form_objects
Decouples your models from forms. Contains validations and nested models.
Complex persistence logic in the form could be combined with service object.
# helpers
Contains reusable methods for views. Should not depend to any particular model.
# mailers
# models
Collection of classes whose purpose is to store and fetch data.
Should represents some storage engine (Mongoid/ROM/ActiveRecord).
Combination of queries, validations, relations, persistence, etc..
# observers
Respond to life cycle callbacks to implement trigger-like behavior outside the original class.
# policies
Regulates how to authorize business rules and which data a user can access.
# presenters
Encapsulate logic related for display purposes. Provides a view specific data as attributes for view.
# query_objects
Encapsulate a complex sql queries from your models/services.
Responsible for returning a result set based on business rules.
# repositories
# searches
Encapsulate search and custom filters functionality.
# serializers
Convert objects into some representation (xml/json) for streaming.
# services
Encapsulate operation with business object via some actions.
Criteria: complex action, multiple models, external service, etc..
This is a place where most of the business logic should be extracted.
# state_objects
Destined for state machine: states, events, transitions.
# sweepers
Terminators of the caching world and responsible for expiring caches when model objects change.
# uploaders
Everything related for file uploading, thumb-processing strategy, etc..
# validators
# value_objects
Simple immutable objects whose equality is dependent on their value rather than an identity.
Allows to combine behavior with the data (example of value objects: Date, Money, PhoneNumber).
# views
# workers
Collection of classes for the tasks performed in the background using background queue library.
