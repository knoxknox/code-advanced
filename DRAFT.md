## App
- api
- cells
- controllers
- decorators
- entities
- exceptions
- form_objects
- helpers
- mailers
- models
- observers
- policies
- presenters
- query_objects
- repositories
- searches
- serializers
- services
- state_objects
- sweepers
- uploaders
- validators
- value_objects
- views
- workers

## DTO lib(s)
PORO, Hashie, Struct, OpenStruct, Virtus, Hamster

## DDD
aggregates, entities, factories, modules, repositories, services, value_objects

## Principles
- DDD
- CQRS
- GRASP
- SOLID

## Books
- http://www.ozon.ru/context/detail/id/4884925/
- http://www.ozon.ru/context/detail/id/5508646/
- http://www.ozon.ru/context/detail/id/5800704/
- http://www.ozon.ru/context/detail/id/20217137/
- http://www.ozon.ru/context/detail/id/21916535/
- http://www.ozon.ru/context/detail/id/30958003/
- http://www.ozon.ru/context/detail/id/31079082/

## Links
- https://github.com/dapi/good_programming
- https://en.wikipedia.org/wiki/GRASP_(object-oriented_design)
- http://blog.byndyu.ru/2014/07/command-and-query-responsibility.html
- http://code.tutsplus.com/tutorials/how-to-write-code-that-embraces-change--net-29716
- http://victorsavkin.com/ddd
- https://speakerdeck.com/skwp/domain-driven-rails
- http://www.slideshare.net/dwhelan/domain-driven-design-and-hexagonal-srchitecture-with-rails
- http://www.slideshare.net/creatop/railsway
- http://blog.lunarlogic.io/2013/declutter-lib-directory/
- http://karolgalanciak.com/blog/2013/10/06/structuring-rails-applications/
- http://blog.codeclimate.com/blog/2012/10/17/7-ways-to-decompose-fat-activerecord-models/

# admin
# api
# calculators
Contains complex calculations for your business rules in isolation.
# cells
Encapsulate parts of your page into separate widgets. Mostly, used in views to replace a helper/partial mess.
# commands
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
# errors
# form_objects
Decouples your models from forms. Contains validations and nested models.
Complex persistence logic in the form could be combined with service object.
# helpers
Contains reusable methods for views. Should not depend to any particular model.
# mailers
# mappers
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
