# CliHelloWorldLazyRollup

This test checks bundle sizes when there is a lazy module and experimentalRollupPass is used. It also checks if the `ngDevMode` global variable and string references in `packages/core/src/util/ng_dev_mode.ts` are correctly removed.

This test contains a lazy route to ensure `ngDevMode` removal happens even across chunks, and a payload size check in `../_payload-limits.json` to ensure extra code is not retained accidentally.