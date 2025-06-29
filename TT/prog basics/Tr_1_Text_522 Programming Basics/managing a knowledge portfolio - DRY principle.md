
The DRY principle: Every piece of knowledge must have a single, unambiguous, authoritative representation within a system.

Duplication we see falls into one of the following categories:
Imposed duplication. Developers feel they have no choice-the environment seems to require duplication.
Inadvertent duplication. Developers don't realize that they are duplicating information.
Impatient duplication. Developers get lazy and duplicate because it seems easier.
Interdeveloper duplication. Multiple people on a team (or on different teams) duplicate a piece of information.

Sometimes, duplication seems to be forced on us. With a bit of ingenuity you can normally remove the need for duplication. Often the answer is to write a simple filter or code generator. Structures in multiple languages can be built from a common metadata representation using a simple code generator

The trick is to make the process active: this cannot be a one-time conversion, or we're back in a position of duplicating data.
