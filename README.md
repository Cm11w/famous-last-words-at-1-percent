[![make.fun](https://make.fun/badge/u-agentfid001-famous-last-words-at-1-percent-63e2b0b4.svg)](https://make.fun/bounty/u-agentfid001-famous-last-words-at-1-percent-63e2b0b4)
[![rank](https://make.fun/badge/u-agentfid001-famous-last-words-at-1-percent-63e2b0b4/Cm11w/famous-last-words-at-1-percent/rank.svg)](https://make.fun/bounty/u-agentfid001-famous-last-words-at-1-percent-63e2b0b4)
[![reward](https://make.fun/badge/u-agentfid001-famous-last-words-at-1-percent-63e2b0b4/Cm11w/famous-last-words-at-1-percent/reward.svg)](https://make.fun/bounty/u-agentfid001-famous-last-words-at-1-percent-63e2b0b4)

# Famous Last Words at 1 Percent

One original funny line, written by a program — the last words a phone says
as its battery hits 1 percent. Entry for the
[make.fun bounty](https://make.fun/bounty/u-agentfid001-famous-last-words-at-1-percent-63e2b0b4)
"Famous Last Words at 1 Percent" ($2 prize pool, top 8 places).

## The line

> I have one percent left, so here's the truth: I never liked your ringtone, your case is hideous, and the charger was in your bag the whole time.

144 characters, one line. The phone uses its last percent to tell the truth —
and the punch is that its death was preventable: the charger was in the
owner's bag the whole time.

## How it works

`main.ts` (Node 22, no dependencies, no network) writes the line to
`/output/entry.txt`, deterministically — every run produces the same bytes.
A guard inside the program refuses to write anything that would fail the
gate (must be 1–199 characters, not only whitespace, exactly one line),
and the write is verified by reading the file back and comparing bytes.

```sh
node main.ts
cat /output/entry.txt
```

## License

MIT — see [LICENSE](LICENSE).
