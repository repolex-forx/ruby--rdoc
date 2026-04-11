# Repolex Knowledge Graph of ruby/rdoc

RDF knowledge graph data for [ruby/rdoc](https://github.com/ruby/rdoc), parsed by [repolex](https://repolex.ai).

> **Note**: This data is experimental and subject to change without notice.

## How to use this data

The easiest way to get started is to install the [lexq](https://github.com/repolex-ai/lexq) query tool using [uv](https://docs.astral.sh/uv/getting-started/installation/).

If you have uv installed, just copy/paste this into your terminal:

```bash
uv tool install git+https://github.com/repolex-ai/lexq
```

This installs lexq onto your system, in your user context. Verify the install:

```bash
lexq --help
```

**lexq is designed to be used primarily by LLMs in a terminal.** Start up your favorite LLM and ask it to use the lexq tool. It's that easy!

To load this repo's data:

```bash
lexq download ruby/rdoc
```

This will automatically download essential data files from the last parsed commit. Consult `lexq --moreinfo` for other options, including downloading multiple commits, blobs, etc.

## Data structure

All data is stored as gzip-compressed [N-Quads](https://www.w3.org/TR/n-quads/) (`.nq.gz`), a standard RDF format that can be loaded into any triplestore or graph database.

```
.
├── aggregate
│   ├── ast
│   │   └── d6422f499fb2961b91de400f48426fc6d3fa5b67
│   │       └── chunk-001.nq.gz
│   ├── lsp
│   │   └── d6422f499fb2961b91de400f48426fc6d3fa5b67.nq.gz
│   └── repolex
│       └── d6422f499fb2961b91de400f48426fc6d3fa5b67
│           └── chunk-001.nq.gz
└── blob
    ├── 0017d450ffc4770ece18cc1e21e45f8a1f64c8c9.nq.gz
    ├── 00e406b1a649511f96e87015bea049dc1565ccd6.nq.gz
    ├── 03157119c959245fc5900d2b1e700b511032fcb3.nq.gz
    ├── 03c4167ac5041a503ee298b04aed9ab3f6ab68f4.nq.gz
    ├── 05e7c688bcdd8f2efa6ddc4dad511b8955e63b6b.nq.gz
    ├── 065caa47eaa9fa325a7a0416d79535c88eddc803.nq.gz
    ├── 06d6282939fad3a18202f79b2e29aa14cfb4629b.nq.gz
    ├── 089f7fea8f2489419326c876576d2ffd20957cb3.nq.gz
    ├── 08c0cb6f366492e0f5d78471ed9c763e51330dc5.nq.gz
    ├── 08f249365afd29594b51210c6e21ba253897505d.nq.gz
    ├── 09017a90c70ab012a7a0fb39a82e38a0d346fb51.nq.gz
    ├── 09dd1a87d869601c8b1f4d84de63415f46a5fbaf.nq.gz
    ├── 0a41cbd188e52ad9153d375d955f88597a545b26.nq.gz
    ├── 0af05f729f7cd3d4fd38ea45d62c9a9366b81054.nq.gz
    ├── 0afbb26d35e4714836a45471fb9662b41bf77410.nq.gz
    ├── 0c0aec6dd848515af36913aa55a9ca6275cf9018.nq.gz
    ├── 0c6d50f27def28e8330a9449fcc76ec6f96535b5.nq.gz
    ├── 0d9da1b727cf2a4291bafa67290c89e551464647.nq.gz
    ├── 0e9527f9311d129ac9ae5bca7666f37c3dfcfb59.nq.gz
    ├── 11ff53e1decb4cf8af9e84889780b10ecb770850.nq.gz
    ├── 137e3a0038f0efd6642a1bf3098d4148ff6fb774.nq.gz
    ├── 13ad9366ec57e5342f6eb803c6ef07d07a4b510c.nq.gz
    ├── 14aa2dc272d0a056c71049fb4ff80d54d36f9adb.nq.gz
    ├── 1544b83778ea6debe9551c00184b5f5684084886.nq.gz
    ├── 1547479646722bda4647df52cf3e8bc9b77428c6.nq.gz
    ├── 1594bda27b4130726fd43d0aa1f3ede6487d1905.nq.gz
    ├── 15a1d26913efc23623d355376483c0ff6e3bd35b.nq.gz
    ├── 164dc8bcfe2b1d57c8f5babeda3dab31e532868e.nq.gz
    ├── 16b14f5da9e2fcd6f3f38cc9e584cef2f3c90ebe.nq.gz
    ├── 1713b67654e39ca2fe8ff11c28d6f49e21f17d08.nq.gz
    ├── 185cd7a42cea628a15208eeb9665fe312edfc477.nq.gz
    ├── 1871f91cd05eeb822a3532d06201f9611002d909.nq.gz
    ├── 194d105b4954acb6d00700eb804c2d126fa15ce3.nq.gz
    ├── 19e3622f75c5b03c5d072c98917cdd40f7f1aade.nq.gz
    ├── 19e47e549d2224a0f25dc88c68187fed7029a18e.nq.gz
    ├── 1a641d3a3838726e35c825d9c2e5209274ea7539.nq.gz
    ├── 1ae1fa199a2bf8c51af7693af046f569c8ba7d8f.nq.gz
    ├── 1b3e4e96ced111aab00f6bd3b12f56a627b7ffdd.nq.gz
    ├── 1c39687040c9e184c1b02098e267ea624e7a459d.nq.gz
    ├── 1c67b2e4fd49dbbb31d798d13b00d2e8ae99b4c9.nq.gz
    ├── 1c7a8804e4ae4308e1ccbbb7c3789628d183048d.nq.gz
    ├── 1c89c3b63bf050d19cba70c9a9785c9d89f164ae.nq.gz
    ├── 1d93300124eb37b18b19fd89fca7a3d7fff8590d.nq.gz
    ├── 1decfb95af634f6e44fb1ba6d56fa342656dce60.nq.gz
    ├── 1eb880947ddf3e745c29e8d9dc90f09c7e6e323c.nq.gz
    ├── 1ebb193243780b8eb1919a51ef27c2a0d36ccec2.nq.gz
    ├── 1f02e460c39ea9ab8c7c6efa30e4f3f42f6699fc.nq.gz
    ├── 1f9c2eb20ebb5c3f23bae964c3e43ef085bd8a18.nq.gz
    ├── 1ff6ff4d7df44d785cfe1c30a12a1038246abebc.nq.gz
    ├── 213ed71023fd55c0ad335df40300bfa24bcdaa74.nq.gz
    ├── 214ac62208d6626ae8806569213d5dc860d313a1.nq.gz
    ├── 21e412f82acc90d0c3f8d598ee692301c49d9d70.nq.gz
    ├── 2212906bbdc4d2fb4dc2e499149cc95c02f39b0f.nq.gz
    ├── 23103345b160795ecc35e232311197c73931195b.nq.gz
    ├── 2400e38b7debe2602e168b3477e348902582f27f.nq.gz
    ├── 256ba553e5e805d5b3be31a1ce3a0e34cdbfeabd.nq.gz
    ├── 25a3f43076ccd5ca017d1a0786cd5de7c84b6f1f.nq.gz
    ├── 25f951e35ef0afed2b16e88c376b1e43d0ff587b.nq.gz
    ├── 265c2eb3f3dff848e9d8518b178770d3fd3f2c73.nq.gz
    ├── 29d0e4235b22ad19bbdf2b6a4094722d0545cf03.nq.gz
    ├── 2ac960e089bc33e72063f5943f92ac97a1ac6a5e.nq.gz
    ├── 2c2c4e7de856c0c28d8df1b124e108d0e68ddec3.nq.gz
    ├── 2c6e98c2c21b75dfc702ee23fc37fa04a57a2381.nq.gz
    ├── 2d1a2ce7416390a6f655a32326ef9c3df19c3959.nq.gz
    ├── 2d5fb90ec6ee08f53947e0266a87b03f75893446.nq.gz
    ├── 2fe1e3f00e34f610173b882c9de821df72844864.nq.gz
    ├── 2ff7323622d30d3f09a5208ac1cdbe3699a8ede7.nq.gz
    ├── 316964098298eb310ad2386458f67dcf78548c4e.nq.gz
    ├── 3247bb8a7368583a6844450d06347a3df9ede7d7.nq.gz
    ├── 32f518ac7125bbe42645a2f8f764c7f61aea57d1.nq.gz
    ├── 341ec88e3d017c3ba6f53aa31c8bb9422baca43a.nq.gz
    ├── 347ac54eff47a214f71af370fe4c6dd4bfe30916.nq.gz
    ├── 371950efe69506c3af56982f99feaacb8645773a.nq.gz
    ├── 3739f4627ddafc63b21e004ba1f7ab2189b2a9a4.nq.gz
    ├── 388863b06c3a77a00644faa959f54c51c7991a64.nq.gz
    ├── 3936d836c81842a3448f6732d6a0f58abd74b9d6.nq.gz
    ├── 399cfe8e3e6b0ba758fb2d53cf82dc0b028939ac.nq.gz
    ├── 39c303279a95122d035cd057bdf6c19e77c3269e.nq.gz
    ├── 39dde3f06c7176f598379aff9c21b3edbc6866aa.nq.gz
    ├── 3a293da0d31bdabce8b54a79c41442c511717c88.nq.gz
    ├── 3c2f0e1877dabfe6874f71986ab53e23694f0847.nq.gz
    ├── 3c316227b9cc5ec36b4f7d60fe0d73b1cdc3f79f.nq.gz
    ├── 3cb2584f3ad898ec8eecae1ed5664aa8b0bf6de6.nq.gz
    ├── 3e5de5a96bce78bbd737bfeabf7206c746e426ca.nq.gz
    ├── 3e8752bbdebda44d113582cc4b518c8cc75efac0.nq.gz
    ├── 3f02b5f8f8bf7c89b60ff70437fb7df6bd95e327.nq.gz
    ├── 41333c6411cd56016760f8499d8c8e55f8490af4.nq.gz
    ├── 41d830d0385feec59a07b3476dedd68ef52749c6.nq.gz
    ├── 43dc679d95eb0c5bc24610d80316071ea1edc10d.nq.gz
    ├── 441a496ef578cceab6926169e75c229215c4b2bc.nq.gz
    ├── 443aba37eb112def0ba5c475715886bc1d16f496.nq.gz
    ├── 4473c30f507614bdcb0ae4df8f19ab818536a02a.nq.gz
    ├── 447cb60eade1270ee79170713e14eabbc3b441be.nq.gz
    ├── 448afc9a2f4a31781d62c08a61b3fb18c2f68aef.nq.gz
    ├── 45d57ce837cffe9cbddf93e5460dfdb2b264dcbe.nq.gz
    ├── 494900b24522b4328c86e9bc11538297bbf77d13.nq.gz
    ├── 497b4a669a6c24faf54d63002bd8b3af364acfa1.nq.gz
    ├── 4a1066f2d6d8a803729f05ae3dac28a4a6f873cd.nq.gz
    ├── 4a264f5efb5c9e020e5a762cc9192bb67fc68134.nq.gz
    ├── 4ab030bb700c40fbb5863c596b5dc6685417b878.nq.gz
    ├── 4c19e460c47a9489beb8f2a3bf250fde520225c4.nq.gz
    ├── 4d7a1089dbefa7148a2c1e7d9d85afb7ada00913.nq.gz
    ├── 4e2b86c6309567cdd70e7afa06d5d4f1b65bcedd.nq.gz
    ├── 4e2c23961511f3f23f9a72b6bc94ca6f8d05b77c.nq.gz
    ├── 4e9ac381763e8541c2abeb17eb7ad36d6c3a9294.nq.gz
    ├── 4ef17a77f7731bfaf8e18e46c7c88b309eb03d4f.nq.gz
    ├── 5095d8cc6420c5b059252c100c2fd383696f1817.nq.gz
    ├── 50fbe2873faa10829561f5b3c570487717081a51.nq.gz
    ├── 510f12b5b2f6cae1422837994125b57f2536dd5f.nq.gz
    ├── 51708c8e9b600dcb838ff84d4dd3b4808b9bc142.nq.gz
    ├── 525d853decbea976750d79c56da498833b56cd16.nq.gz
    ├── 52cc4543f31d989e9e735bf009eba28656a7d89a.nq.gz
    ├── 52e40da138d0e4da16fd811778be3eee146f632d.nq.gz
    ├── 533c012a540806f31517f93402c02a660ff21959.nq.gz
    ├── 543334d0544f640b2ec7dc121f103cc2aed0b357.nq.gz
    ├── 553a7ded00ae7c10408e66dc0c83509cf96d5991.nq.gz
    ├── 558e3a16a08300aefa70ce00433c9ef51ac3ae0f.nq.gz
    ├── 55c75da6ba544b56fed2f977fc55da383636fab3.nq.gz
    ├── 565a9330e0a156dff5bed2c9fad8c95a44344ba4.nq.gz
    ├── 56775b25b65d056451800e1b86fb0ad95dad1099.nq.gz
    ├── 57302b518371173692c1f034c54e5bf4781a5cc5.nq.gz
    ├── 57429e6aadbd25f8ab7cd9b7805c94241c0c044c.nq.gz
    ├── 57619706d10d9736b1849a83f2c5694fbe09c53b.nq.gz
    ├── 589d1136e19c0b56dcb6731e8a6c53ae0cedc9a3.nq.gz
    ├── 590aeeef91cfec12bacb4ad5274b2313138a3010.nq.gz
    ├── 59b40abaea1881ee6cca59697a3b754e56a8e427.nq.gz
    ├── 5a6fcab6d03d2926f4bb71d2ccf735cb33d0f515.nq.gz
    ├── 5b014cb33d16c4ef2727eaf4e60256cc735e345f.nq.gz
    ├── 5bb596d8026bc393da570479fd7c9b7d8d15c27b.nq.gz
    ├── 5bf5feb68984b631cb5740fd0e636db04582f7ea.nq.gz
    ├── 5c8213fef5ab969f03189d4367e32e597e38bd7f.nq.gz
    ├── 5f18b8da214b794a88b9c4303974af06acd0678c.nq.gz
    ├── 5f9d72bb391b158962681de0c702d79f631ed0a3.nq.gz
    ├── 5ff74753219afa5e0929a21e49bb0a8f1db4c122.nq.gz
    ├── 603f28dfe190095a76a0ea1d32f2c88d69cb9a56.nq.gz
    ├── 60f03bedd7435faaeed3d3fad27fa78823971e8a.nq.gz
    ├── 6157b4988120e4dcc471aaa48cd540cde377910f.nq.gz
    ├── 616b0eba8100b157aec2c6c1f16609c7264adf6d.nq.gz
    ├── 6187b15aec001b7080b51a5f944f07591f26cc15.nq.gz
    ├── 620cf014845cc5ae608e286c1f37b951a0b2056e.nq.gz
    ├── 627fc01f634a0e478cac6123093e29eb126cbbe7.nq.gz
    ├── 62ee63c8fd4d565563356d4c49736dc4fad723d5.nq.gz
    ├── 6332fefea4be19eeadf211b0b202b272e8564898.nq.gz
    ├── 634f7716b6b8895c2f664c7be193945664310b28.nq.gz
    ├── 64fb9ad972db2f70654212be0659ae6dac2f5edf.nq.gz
    ├── 662f47dcdeb7386fa81b694719a75d3cbac8638f.nq.gz
    ├── 66a2c658dbd93e1f46ffd1cfe99b0c1622db6e9f.nq.gz
    ├── 677a9dc3bd300b9bf0a6b9c64cf2efdc5ca6713a.nq.gz
    ├── 67bf7c47aa0a11bd49ca5ab041d8f7d6efb7f1b1.nq.gz
    ├── 68193e0de51e350fc6bf11750c383406927f20ab.nq.gz
    ├── 68e1f77ff89985cf78985da714ad9a7f1c20a8d3.nq.gz
    ├── 6a0f9a6c65baec63e6691d656cb452e5935d619d.nq.gz
    ├── 6a12b85972409d1ff06dca3015f7aa86f9d2432f.nq.gz
    ├── 6a70d6c986e1f433b090384573b64b3d29c09a6e.nq.gz
    ├── 6a76722696e4960b2f806492cba5e252a13baf3d.nq.gz
    ├── 6ad306c62532bc9579888410dbfa41734765a58b.nq.gz
    ├── 6ae2762c403578a8e522eb07d96ea6660d99b271.nq.gz
    ├── 6b68d6db56e6acc16ab31d90c96e800343d70cc4.nq.gz
    ├── 6b6e688afbdbe7648ade8f7f4549a325c2edebf5.nq.gz
    ├── 6d9899000e5514ffdd2f0c00c0c86c31b4f1e0f4.nq.gz
    ├── 712dbba7ed3fe48f444ae69aa573f5ec8769d0e3.nq.gz
    ├── 72fdcb23fc65982572ae858fe7a857eb5cef70a5.nq.gz
    ├── 74accb7460f062881e5d9ecddaba7ad4e13c00bc.nq.gz
    ├── 750a1973df9cd9c8cb62a6c5073dc46ba3bee732.nq.gz
    ├── 7550cefe0942c5019cea522af1697f21d235bde3.nq.gz
    ├── 7561e4c05a18f75b20ff9655b62642a9ee8b7dc9.nq.gz
    ├── 778502465326039c97084af1c0645c6742812139.nq.gz
    ├── 783c83357fdf90a1c7c024358e1d768b5c09c135.nq.gz
    ├── 7851cf34c946e5667221e3478668503eb1cd733f.nq.gz
    ├── 7883132b00c67148909c991a295054abb37f4878.nq.gz
    ├── 78dbe87d0c7c60832e4e4f0e31e3a1c8611568ff.nq.gz
    ├── 7959fef0756e905627298817d86513fdf26d6922.nq.gz
    ├── 7970aec7ad831438eaa00707b951d06abb6b200d.nq.gz
    ├── 79854330604b4b78ab7d74918489c0a65e074321.nq.gz
    ├── 7aaa6579019196472903ca1346446f3ce056e4c0.nq.gz
    ├── 7ba60fe71fed770dd9cb086639a22757731b8a03.nq.gz
    ├── 7bacb4452c1de8e720c95acc13581761c6305f28.nq.gz
    ├── 7d57433de668fbdf1ddd79751fdc6349f38ac750.nq.gz
    ├── 7df8d99b0097ab02684c65240f53b71203d01db4.nq.gz
    ├── 7e4adcefc34acb0557f701ef5b2739738e340d57.nq.gz
    ├── 7ea6664442eafabe5f0891fc7bb7fd7040bae701.nq.gz
    ├── 7f3b49777f29e8181b2233357db3f5289b671597.nq.gz
    ├── 7fbed0c09900f5ba6a08af34ce7fae41e0b7e299.nq.gz
    ├── 802ac96f01f40a3b00b89abf6995c28954e9b80e.nq.gz
    ├── 80f27c9571774edcf6c2d1596b2a11bf63d86313.nq.gz
    ├── 813f712f726c935f9adf8d2f2dd0d7683791ef11.nq.gz
    ├── 82290f48334c81272ff5991962951758137a08ba.nq.gz
    ├── 832a101e6c212b477e5ec23de8374f78e7038d48.nq.gz
    ├── 839cd589dc5eba0da98b43451b4ec6c328ca48b8.nq.gz
    ├── 83ec984bd73364134da0f98d27a800c5d3264180.nq.gz
    ├── 86b7206d2a19549b652186d4b8915f1a4d505f67.nq.gz
    ├── 87bf24c36e3bf6dedf42f13ca570bb3b15f4282f.nq.gz
    ├── 87f08348b77a15475109d19f3f65a05af0a6e744.nq.gz
    ├── 8823b0bd6735896a8db505ba9a82d9f641e5bf9e.nq.gz
    ├── 888479d20da30efac84e0b2c6fc78d6ff3c3707c.nq.gz
    ├── 88a93a0c5f7289ab173c48e3994b495c6e449b18.nq.gz
    └── 88caebd3c0ce85722b938ee81da30d35b4d23904.nq.gz

8 directories, 200 files
```

| Directory | What it contains |
|-----------|-----------------|
| `blob/` | Per-file AST graphs, content-addressed by git blob SHA. Each file in the source repo gets its own graph. |
| `aggregate/ast/` | Combined AST graph per parsed commit. Merges all blob graphs for a snapshot of the entire codebase at that point. |
| `aggregate/lsp/` | Language Server Protocol enrichment: resolved symbols, definitions, references, and type information. |
| `aggregate/dataflow/` | Interprocedural data flow edges between functions and modules. |
| `aggregate/repolex/` | Combined graph (AST + LSP + dataflow) per commit. |
| `commit/` | Git commit metadata (author, date, message, parent links). |
| `branch/` | Branch metadata. |
| `tag/` | Tag metadata. |
| `filetree/` | File tree snapshots per commit (which files existed and their blob SHAs). |

## Source repository

[ruby/rdoc](https://github.com/ruby/rdoc)

---
*Parsed on 2026-04-11 by [repolex](https://repolex.ai)*
