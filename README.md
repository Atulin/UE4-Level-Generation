![](https://thumbs.gfycat.com/TheseNegligibleKodiakbear-size_restricted.gif)
*Each of the rooms you see is a level instance. Spawning speed - real time.*

# Level generation demo

This level generation is based on **level instances** instead of actors as the main level rooms. This allows the user to use the level editor to edit rooms, instead of having to put up with the Actor editor. It's made entirely in **Blueprint**.

I have decided to release it in its sorry state as my open-source contribution to the Unreal Engine 4 community, maybe together we can make it fully work. It's one of my oldest projects, if not the oldest, so there is some issues with it:

1. The spawning algorithm relies on ``Delay`` nodes. Heavily. I couldn't make it work without them for whatever reason.
2. The algorithm is also inefficient. Sometimes rooms simply don't spawn, so it goes over the possible locations multiple times.
3. I didn't come up with a way to allow level switching. As in, you finish a floor and go to the next one.

There's also some issues that stem from the sole fact of it being one of my first UE4 endeavours:

1. Graphs are messy and barely use Macros, Functions and the like
2. Folder and file structure is garbage

But I sincerely hope, that with the help of our community we can make it work, for our common benefit. It's *this* close from being done, after all.
____

## License

``Mozilla Public License 2.0``
____

## Documentation

* Start from the ``Room1`` level. Teleporting there from ``PersistentLevel`` fails ¯\\\_(ツ)_/¯
* All the relevant actors sit in ``Utilities`` folder
  * Room Spawner Probe – calculates which room to spawn and spawns it
  * Floor Master – manages the probes

____

## Changelog

* 05.08.2018
  * added some comments to the graphs
  * Replaced a sequence with custom events
