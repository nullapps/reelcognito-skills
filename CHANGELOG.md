# Reviewed releases

## muse-v5-r2 · November 26, 2026

Packaging revision 2 places the [Muse skill](skills/muse/reelcognito-mystery-movie-nights/SKILL.md) in a folder matching its frontmatter name. The four reviewed v5 artifacts retain the SHA-256 values below. Installation verifies five pinned files and ends. A separate first-use request starts the interview, secure connection setup and live compatibility preflight.

## muse-v5 · November 26, 2026

First official Muse distribution. The combined v5 instructions and standalone main prompt retain their reviewed bytes. The compatibility companion ends at its closing COPY marker. Both customer COPY blocks occur verbatim in the combined file. V5 includes the one-time token provisioning steps and checks the immediately preceding theatrical release for sequels and prequels. The YAML snapshot records the published revision 7, version 2026-11-21.2.

| Artifact filename | SHA-256 |
| --- | --- |
| reelcognito-agent-setup-prompt-v5.md | `c786798ebbca348395a4afc4722f556b50af8d3910346df4aa8767f68e10668c` |
| reelcognito-agent-patches-setup-v5.md | `dce53115a6f3c0b0212bdddbbb55096ca1751a06d0a078d5c3b27c65d886c39a` |
| reelcognito-agent-patches-v5.yaml | `41dc3609f5d9a62f156be41e3b741935b1ec6c22010ebf78bb2acda6f170c9c8` |
| reelcognito-agent-setup-combined-v5.md | `4a0a1300b38111309da3f9cc9b58e9f14936ffe10e44849028cd8de0246d4e4f` |

## Publishing the next reviewed release

1. Start with the approved instruction package and its independent release record. Compare the combined file byte-for-byte with the website's canonical download and checksum. Compare the component COPY blocks with the combined file. Resolve any newer website release before packaging. [Canonical download](https://reelcognito.com/agent-setup.md)
2. Stage only the approved public paths. Review each file, including text outside the COPY markers. Exclude publisher materials. Capture the reviewed, approved public manifest bytes for the release snapshot. Record the source and public digests where a customer extract differs.
3. Validate the folder name against frontmatter, Markdown, YAML, checksums and references. Test static installation with access limited to the five pinned downloads. Exercise setup and failure handling in isolation. Scan the release tree and the Git history to be published for secrets and private information.
4. Commit and tag the reviewed tree. Resolve the tag to a full commit SHA, then build the installer outside the commit with the exact raw URL and SHA-256 of each installation file. Retrieve every URL anonymously and compare the bytes. Include the installer in the release notes.
5. Run clean-Muse acceptance before submitting the new pin for directory review. For a correction, publish a new reviewed commit and tag. Existing installations update with customer approval. Compatibility updates continue through the live feed.
