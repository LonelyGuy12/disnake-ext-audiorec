Usage
=====

This voice implementation operates
using the disnake ``VoiceProtocol`` interface.

To use it, pass the class into
`VoiceChannel.connect <https://disnake.readthedocs.io/en/latest/api.html#disnake.VoiceChannel.connect>`_

.. code-block:: python3

    from disnake.ext.audiorec import NativeVoiceClient

    # ...
    client = await voice_channel.connect(cls=NativeVoiceClient)

    client.record()

    await asyncio.sleep(30)

    audio_binaries = await client.stop_record()


For other examples, please see the
`examples folder <https://github.com/LonelyGuy12/disnake-ext-audiorec>`_
on GitHub.
