# Nostr Voice Chat

## Proof of Concept

There is a million apps that let you voip to random strangers and this is just
a proof of concept, doing the same with
https://github.com/nostr-protocol/nostr.

It uses https://github.com/fiatjaf/nostr-tools and 90 lines of custom code to
provide a simple multi party voice chat client relying on nostr relays.

Those relays currently are almost all providing the "pipes" for free to store
and forward messages. This tool here opts out from storing relatively big
messages. In fact the messages are probably too big for most relays but
relay.nostr.info for now does forward bigger messages for ephemeral messages.

This software can be used under the MIT license.

This software can be tried out [here](https://relay.nostr.info/test/chat.html).

Please be aware that as of now, the connection randomly breaks a lot and
reconnects are delayed more with every disconnect, so for your test, hit reload
if you notice a lost connection.

**Warning**: This tool publishes your audio "to the world" with no encryption.