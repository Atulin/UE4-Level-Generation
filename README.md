# Level generation demo

This level generation is based on **level instances** instead of actors as the main level rooms. This allows the user to use the level editor to edit rooms, instead of having to put up with the Actor editor.

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

I haven't picked one that's fully suitable for the project **yet**. But here are some basic guidelines:

1. If you make some improvement to this system, please, share. Don't keep it to yourself only.
2. You can use it for commercial or non-commercial games, as you wish.
3. Your end product can have whatever license you wish it to have. The level generation system, however, should have at least an open source. Or, preferably, it should make it as a push request to this repo here.
4. Credit is not necessary, although appreciated.

In the end, the license will probably be ``Mozilla Public License 2.0``, but it's not guaranteed quite yet.
____

## Documentation

None yet. Will probably be created. Some day. In the meantime, feel free to open issues to ask for stuff.