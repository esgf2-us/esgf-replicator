# Open Questions in the ESGF-NG Replicator Design

* Can we use topics on the event stream to limit what the Replicator sees to what it needs?
* What topics will the event stream have?
* Can we count on an event stream that has all events forever?
  * For this design to work, it assumes it can get all events that have ever been published. If that’s not true, we need to provide another way (beyond subscribing to events) to “catch up” with previously published things
* Do we need to support anonymous HTTPS access as an allowed method for MVP?
  * It’s costly, so if we can avoid it, we should.
* How many Replicators (i.e., event stream subscribers) are we prepared to support?
* If the event stream materializes events and updates are consolidated (such that consumers don’t see an original publish and later update), how will the Replicator be able to know when a dataset it’s previously replicated needs to be updated or not? Does the STAC item’s  version number help us detect this?
* Does the replicator need to subscribe to (or act on) update events?
* Does the replicator need to subscribe to (or act on) retractions?
