# Announcements for Kazoo

This file will serve as a reference point for upcoming announcements, both of the temporal nature (this library will be deprecated in 6 months) and version-specific (upgrading from X to Y will require A, B, and C).

## Upcoming

### May 2016

#### Deprecating `deps/mochiweb`

Most operations have been moved to the Cowboy or Cowlib projects. We will formally remove mochiweb from `deps/`. If you maintain code apart from Kazoo that uses mochiweb, please either covert to equivalent functionality with Cowboy/Cowlib or plan how you'll build your custom code with your own dependency of mochiweb.

#### Replacing `deps/exmpp`

exmpp library has problems restarting. it will be replaced by `deps/escalus`

## Versions

### 4.0

#### Number Manager

Upgrading to 4.0 will shift number management from `core/whistle_number_manager` to `core/kazoo_number_manager`. The upgrade process *should* be seamless from the user's perspective.

#### CouchDB

Upgrading will change the way Kazoo interacts with CouchDB (including deprecating using BigCouch and recommending CouchDB!). For most operations, nothing will be noticably different.
