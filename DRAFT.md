## Structs (DTO)
PORO, Hashie, Struct, OpenStruct, Virtus, Hamster

## Principles
- DDD
- CQRS
- GRASP
- SOLID

# api
- https://github.com/bogdan/datagrid
- https://github.com/ruby-grape/grape
- https://github.com/mavenlink/brainstem

# cells
Encapsulate parts of your page into separate widgets. Mostly, used in views to replace a helper/partial mess.
- https://github.com/apotonick/cells

# controllers
Everything related to parsing requests, sessions, protection, rendering templates, redirecting, flash messages.
- https://github.com/amatsuda/kaminari
- https://github.com/plataformatec/responders
- https://github.com/josevalim/inherited_resources

# decorators
Allows functionality to be divided between classes with unique areas of concern.
Behavior could be added to an individual object, without affecting the original object.
For example you can wrap your models to extract presentation related logic from helpers.
- https://github.com/drapergem/draper

# dto
Represents data as definite structures that carries data between processes.
Does not have any behavior, manipulates data only via accessors and mutators.
- https://github.com/solnic/virtus

# entities

# form_objects
Decouples your models from forms. Contains validations and nested models.
Complex persistence logic in the form could be combined with service object.
- https://github.com/apotonick/reform
- https://github.com/GCorbel/activeform-rails

# helpers
Contains reusable methods for views. Should not depend to any particular model.

# mailers

# models
Collection of classes whose purpose is to store and fetch data.
Should represents some storage engine (Mongoid/ROM/ActiveRecord).
Combination of queries, validations, relations, persistence, etc..

# observers
Respond to life cycle callbacks to implement trigger-like behavior outside the original class.
- https://github.com/krisleech/wisper

# policies
Regulates how to authorize business rules and which data a user can access.
- https://github.com/elabs/pundit

# presenters
Encapsulate logic related for display purposes. Provides a view specific data as attributes for view.
- https://github.com/rf-/keynote

# query_objects
Encapsulate a complex sql queries from your models/services.
Responsible for returning a result set based on business rules.
- https://github.com/jeremyevans/sequel
- https://github.com/samleb/sexy_scopes
- https://github.com/activerecord-hackery/squeel

# repositories

# searches
Encapsulate search and custom filters functionality.
- https://github.com/toptal/chewy
- https://github.com/nathanl/searchlight
- https://github.com/RStankov/SearchObject

# serializers
Convert objects into some representation (xml/json) for streaming.
- https://github.com/amatsuda/jb
- https://github.com/rails-api/active_model_serializers

# services
Encapsulate operation with business object via some actions.
Criteria: complex action, multiple models, external service, etc..
This is a place where most of the business logic should be extracted.

# state_objects
Destined for state machine: states, events, transitions.
- https://github.com/aasm/aasm
- https://github.com/pluginaweek/state_machine

# sweepers
Terminators of the caching world and responsible for expiring caches when model objects change.

# uploaders
Everything related for file uploading, thumb-processing strategy, etc..
- https://github.com/carrierwaveuploader/carrierwave

# validators
- https://github.com/kodio/veto
- https://github.com/hanami/validations
- https://github.com/jamesbrooks/hash_validator

# value_objects
Simple immutable objects whose equality is dependent on their value rather than an identity.
Allows to combine behavior with the data (example of value objects: Date, Money, PhoneNumber).
- https://github.com/dkubb/adamantium

# views

# workers
Collection of classes for the tasks performed in the background using background queue library.
- https://github.com/chaps-io/gush
- https://github.com/mperham/sidekiq
