# Timestamping log for `diversity.zeitgitter.net`

This lists all commit IDs for which
[`diversity.zeitgitter.net`](https://diversity.zeitgitter.net) (previously
known as `diversity.enotar.ch`) has ever issued a timestamp
signature. If there are any other signatures, please do consider them invalid.

This is part of the *Zeitgitter* distributed timestamping system. Please learn more
about Zeitgitter at https://zeitgitter.net .

# Verify timestamping log

To verify whether a given commit is in there, e.g., one dated at `2019-04-01
19:30`, please use the following commands on a checked-out copy of this repository:

```sh
git checkout `git rev-list --since="2019-04-01 19:30" --reverse master | head -1`
```

You should be able to find the commit ID in `hashes.log` then.

# Outages

- **2023-10-04 in the minutes after 23:46:20 to about 2023-10-10 10:40 UTC**: A
  full operating system partition caused operations to cease. As the places
  used to store timestamping data were not affected, I assume that no
  timestamps were issued without being duly recorded. (Also, no timestamps were
  issued during the outage itself, so nothing needed recording. Timestamps
  issued between 23:46:20 and the outage (at most 10 minutes later) were
  cross-timestamped only after service resumption.)

