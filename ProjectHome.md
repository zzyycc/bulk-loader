ATTENTION: this project has been migrated to github  at http://github.com/arthur-debert/BulkLoader .

Please, use the issue tracker there, as well as source and dowloads.



BulkLoader is a minimal library written in Actionscript 3 (AS3) that aims to make loading and managing complex loading requirements easier and faster. BulkLoader takes a more dynamic, less architecture heavy aproach. Few imports and making heavy use of AS3's dynamic capabilities, BulkLoader has a one-liner feel that doesn't get in your way.

BulkLoader hides the complexity of loading different data types in AS3 and provides a unified interface for loading, accessing and events notification for different types of content.

This library is licensed under an open source MIT license.
Features:
  * Connection pooling.
  * Unified interface for different loading types.
  * Unified progress notification.
  * Events for individual items and as groups.
  * Priority
  * Stop and resuming individually as well as in bulk.
  * Cache management.
  * Statistics about loading (latency, speed, average speed).
  * Various kinds on progress indication: ratio (items loaded / items to load), bytes , and weighted percentage.
  * Configurable number of retries.
  * Configurable logging.
  * Various assest types (XML, NetStreams, Swfs, Images, Sound, Text Files)

Design goals:
  * Minimal imports.
  * Few method to learn.
  * Consistent interface, regardless of content type.

BulkLoader gracefully handles progress notification in these use cases:
  * Few connections to open: bytes total can be used instantly.
  * Many connections opened: progress by ratio
  * Many connections opened for data of widely varying sizes: progress by weight.