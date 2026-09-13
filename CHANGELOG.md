# BazChat Changelog

## 006 — NPC chat works again

**NPC say and yell lines show up again.** Since patch 12.1 those lines
were silently dropped and the error log filled with "secret value" and
"cannot be accessed while tainted" messages. BazChat's windows now hand
message processing to Blizzard's own chat code, which is allowed to read
the protected data, so the lines display normally, complete with their
timestamps and gutter bars.

One limit remains, set by Blizzard: NPC lines can't be kept in BazChat's
saved history, so they won't reappear after a reload.
