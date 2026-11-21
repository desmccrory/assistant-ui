## aui-perf nightly record

_3 points · 2026-11-19T04:31:14.259Z to 2026-11-21T04:29:01.456Z · latest runner: AMD EPYC 9V74 80-Core Processor · Node v26.13.0_

| bench | latest | Δ7d | Δ30d | min | max | points |
| --- | ---: | ---: | ---: | ---: | ---: | ---: |
| accumulator › assistant-stream: raw controller enqueue overhead › 10,000 chunks from one source stream | 672.08µs |  |  | 556.28µs | 864.27µs | 3 |
| accumulator › assistant-stream: raw controller enqueue overhead › 10,000 controller.enqueue calls | 977.01µs |  |  | 792.74µs | 1.209ms | 3 |
| accumulator › assistant-stream: same 4000-char text, chunk size A/B › 16 deltas × 250 chars | 44.13µs |  |  | 35.63µs | 58.22µs | 3 |
| accumulator › assistant-stream: same 4000-char text, chunk size A/B › 250 deltas × 16 chars | 512.00µs |  |  | 389.91µs | 666.48µs | 3 |
| accumulator › assistant-stream: same 4000-char text, chunk size A/B › 4000 deltas × 1 char (per-token) | 7.951ms |  |  | 6.020ms | 10.380ms | 3 |
| accumulator › assistant-stream: stream + accumulator per-delta cost (16-char deltas) › 100 deltas | 214.68µs |  |  | 163.68µs | 282.75µs | 3 |
| accumulator › assistant-stream: stream + accumulator per-delta cost (16-char deltas) › 1000 deltas | 2.014ms |  |  | 1.474ms | 2.627ms | 3 |
| accumulator › assistant-stream: stream + accumulator per-delta cost (16-char deltas) › 4000 deltas | 7.848ms |  |  | 5.943ms | 10.360ms | 3 |
| accumulator › assistant-stream: stream round trip baseline, no accumulator › 100 deltas | 8.02µs |  |  | 6.33µs | 10.11µs | 3 |
| accumulator › assistant-stream: stream round trip baseline, no accumulator › 1000 deltas | 66.73µs |  |  | 53.44µs | 83.38µs | 3 |
| accumulator › assistant-stream: stream round trip baseline, no accumulator › 4000 deltas | 261.03µs |  |  | 210.59µs | 327.66µs | 3 |
| ai-sdk-system-metadata › ai-sdk: system-message metadata conversion through the runtime › 128 parts, distinct providers (stress) | 80.17µs |  |  | 54.60µs | 107.40µs | 3 |
| ai-sdk-system-metadata › ai-sdk: system-message metadata conversion through the runtime › 16 parts, one repeated provider | 42.08µs |  |  | 30.52µs | 65.03µs | 3 |
| ai-sdk-system-metadata › ai-sdk: system-message metadata conversion through the runtime › 2 parts, one repeated provider | 41.66µs |  |  | 31.57µs | 63.42µs | 3 |
| ai-sdk-system-metadata › ai-sdk: system-message metadata conversion through the runtime › 512 parts, distinct providers (stress) | 243.47µs |  |  | 200.72µs | 318.13µs | 3 |
| ai-sdk-toolkit › ai-sdk: convert fresh AISDKToolkit schemas › 10 static tools | 52.60µs |  |  | 45.77µs | 77.43µs | 3 |
| ai-sdk-toolkit › ai-sdk: convert fresh AISDKToolkit schemas › 100 static tools | 524.38µs |  |  | 479.31µs | 698.64µs | 3 |
| ai-sdk-toolkit › ai-sdk: reuse converted AISDKToolkit schemas › 10 static tools | 7.44µs |  |  | 6.34µs | 10.45µs | 3 |
| ai-sdk-toolkit › ai-sdk: reuse converted AISDKToolkit schemas › 100 static tools | 60.62µs |  |  | 53.75µs | 82.65µs | 3 |
| data-stream › assistant-stream: data stream decode (16-char deltas) › 100 deltas | 583.89µs |  |  | 440.94µs | 732.11µs | 3 |
| data-stream › assistant-stream: data stream decode (16-char deltas) › 1000 deltas | 4.978ms |  |  | 3.741ms | 5.932ms | 3 |
| data-stream › assistant-stream: data stream decode (16-char deltas) › 4000 deltas | 19.642ms |  |  | 14.585ms | 23.420ms | 3 |
| data-stream › assistant-stream: data stream encode (16-char deltas) › 100 deltas | 285.41µs |  |  | 208.30µs | 359.72µs | 3 |
| data-stream › assistant-stream: data stream encode (16-char deltas) › 1000 deltas | 2.755ms |  |  | 2.025ms | 3.455ms | 3 |
| data-stream › assistant-stream: data stream encode (16-char deltas) › 4000 deltas | 10.866ms |  |  | 8.167ms | 13.626ms | 3 |
| external-message-conversion › core: cached external message conversion, one streaming delta › 1000 messages, 6-part replies | 216.76µs |  |  | 204.94µs | 286.73µs | 3 |
| external-message-conversion › core: cached external message conversion, one streaming delta › 5000 messages, 20-part replies | 1.388ms |  |  | 1.388ms | 2.175ms | 3 |
| external-message-conversion › core: external message reasoning continuations › 100 matches | 50.11µs |  |  | 42.55µs | 69.92µs | 3 |
| external-message-conversion › core: external message reasoning continuations › 1000 matches | 505.50µs |  |  | 431.05µs | 710.18µs | 3 |
| external-message-conversion › core: external message reasoning continuations › 5000 matches | 2.689ms |  |  | 2.327ms | 3.843ms | 3 |
| external-message-conversion › core: external message tool results › 100 matches | 59.74µs |  |  | 53.98µs | 76.59µs | 3 |
| external-message-conversion › core: external message tool results › 1000 matches | 601.38µs |  |  | 546.21µs | 781.90µs | 3 |
| external-message-conversion › core: external message tool results › 5000 matches | 3.147ms |  |  | 2.830ms | 4.273ms | 3 |
| external-message-conversion › core: external message unique tool calls › 100 matches | 31.16µs |  |  | 28.10µs | 40.30µs | 3 |
| external-message-conversion › core: external message unique tool calls › 1000 matches | 296.34µs |  |  | 268.02µs | 396.22µs | 3 |
| external-message-conversion › core: external message unique tool calls › 5000 matches | 1.622ms |  |  | 1.422ms | 2.193ms | 3 |
| from-thread-message-like › core: fromThreadMessageLike text parts › 1 text parts | 0.21µs |  |  | 0.18µs | 0.27µs | 3 |
| from-thread-message-like › core: fromThreadMessageLike text parts › 10 text parts | 0.37µs |  |  | 0.30µs | 0.47µs | 3 |
| from-thread-message-like › core: fromThreadMessageLike text parts › 100 text parts | 2.11µs |  |  | 1.59µs | 2.47µs | 3 |
| from-thread-message-like › core: fromThreadMessageLike tool calls › 1 tool calls | 0.48µs |  |  | 0.38µs | 0.68µs | 3 |
| from-thread-message-like › core: fromThreadMessageLike tool calls › 10 tool calls | 2.44µs |  |  | 2.32µs | 3.51µs | 3 |
| from-thread-message-like › core: fromThreadMessageLike tool calls › 100 tool calls | 22.48µs |  |  | 20.09µs | 30.61µs | 3 |
| interactable-array-patches › core: id-keyed interactable array patches › 1000 items and patches | 111.19µs |  |  | 111.19µs | 150.94µs | 3 |
| interactable-array-patches › core: id-keyed interactable array patches › 5000 items and patches | 597.75µs |  |  | 597.75µs | 847.87µs | 3 |
| markdown-preprocess › react-markdown: preprocess › escapeCurrencyDollars, 20,000 tilde runs on one line | 2.117ms |  |  | 1.951ms | 2.735ms | 3 |
| markdown-preprocess › react-markdown: preprocess › escapeCurrencyDollars, 20,000 tildes after prose | 160.86µs |  |  | 118.35µs | 186.13µs | 3 |
| markdown-preprocess › react-markdown: preprocess › escapeCurrencyDollars, 20,000 triple-backtick spans on one line | 2.749ms |  |  | 2.524ms | 3.695ms | 3 |
| markdown-preprocess › react-markdown: preprocess › escapeCurrencyDollars, 5,000 code spans in one paragraph | 355.98µs |  |  | 336.49µs | 513.75µs | 3 |
| markdown-preprocess › react-markdown: preprocess › escapeCurrencyDollars, mixed message, 100 sections | 498.64µs |  |  | 498.64µs | 695.42µs | 3 |
| markdown-preprocess › react-markdown: preprocess › normalizeMathDelimiters, 20,000 tilde runs on one line | 5.643ms |  |  | 5.643ms | 7.351ms | 3 |
| markdown-preprocess › react-markdown: preprocess › normalizeMathDelimiters, 20,000 tildes after prose | 760.52µs |  |  | 483.83µs | 797.35µs | 3 |
| markdown-preprocess › react-markdown: preprocess › normalizeMathDelimiters, 20,000 triple-backtick spans on one line | 16.251ms |  |  | 14.833ms | 23.646ms | 3 |
| markdown-preprocess › react-markdown: preprocess › normalizeMathDelimiters, 5,000 code spans in one paragraph | 2.725ms |  |  | 2.337ms | 3.956ms | 3 |
| markdown-preprocess › react-markdown: preprocess › normalizeMathDelimiters, mixed message, 100 sections | 1.931ms |  |  | 1.766ms | 2.700ms | 3 |
| markdown-streaming › react-markdown: one token after an unchanged fenced code block › 10 KB fenced Markdown | 2.304ms |  |  | 1.986ms | 2.948ms | 3 |
| markdown-streaming › react-markdown: one token after an unchanged fenced code block › 10 KB fenced Markdown deferred | 2.488ms |  |  | 2.194ms | 3.215ms | 3 |
| markdown-streaming › react-markdown: one token after an unchanged fenced code block › 100 KB fenced Markdown | 16.940ms |  |  | 13.415ms | 20.559ms | 3 |
| markdown-streaming › react-markdown: one token after an unchanged fenced code block › 100 KB fenced Markdown deferred | 17.991ms |  |  | 14.668ms | 21.700ms | 3 |
| markdown-streaming › react-markdown: one token changed in the last paragraph, by message length › 1 paragraphs | 1.025ms |  |  | 1.025ms | 1.466ms | 3 |
| markdown-streaming › react-markdown: one token changed in the last paragraph, by message length › 10 paragraphs | 2.120ms |  |  | 1.946ms | 3.042ms | 3 |
| markdown-streaming › react-markdown: one token changed in the last paragraph, by message length › 50 paragraphs | 7.445ms |  |  | 6.479ms | 10.109ms | 3 |
| markdown-streaming › react-markdown: the same token with defer on › 1 paragraphs deferred | 1.468ms |  |  | 1.187ms | 1.468ms | 3 |
| markdown-streaming › react-markdown: the same token with defer on › 10 paragraphs deferred | 1.422ms |  |  | 1.422ms | 1.928ms | 3 |
| markdown-streaming › react-markdown: the same token with defer on › 50 paragraphs deferred | 4.171ms |  |  | 3.698ms | 4.642ms | 3 |
| react-langgraph › react-langgraph: streamed tool argument accumulation › 1000 character argument in 16-character deltas | 252.97µs |  |  | 194.97µs | 345.80µs | 3 |
| react-langgraph › react-langgraph: streamed tool argument accumulation › 10000 character argument in 16-character deltas | 2.089ms |  |  | 1.670ms | 2.851ms | 3 |
| react-langgraph › react-langgraph: streamed tool argument accumulation › 500 short object entries in 16-character deltas | 211.695ms |  |  | 184.701ms | 312.966ms | 3 |
| react-langgraph › react-langgraph: streamed tool argument accumulation › 50000 character argument in 16-character deltas | 10.357ms |  |  | 8.337ms | 13.543ms | 3 |
| react-pi-message-projection › react-pi: streaming tail projection › 10 stable messages | 1.78µs |  |  | 1.21µs | 2.32µs | 3 |
| react-pi-message-projection › react-pi: streaming tail projection › 1000 stable messages | 8.90µs |  |  | 5.40µs | 10.68µs | 3 |
| react-pi-message-projection › react-pi: streaming tail projection › 5000 stable messages | 34.92µs |  |  | 25.73µs | 48.04µs | 3 |
| sse-fragmentation › assistant-stream: fragmented SSE events › 100 KiB, 1 chunks | 7.33µs |  |  | 4.71µs | 7.33µs | 3 |
| sse-fragmentation › assistant-stream: fragmented SSE events › 100 KiB, 101 chunks | 19.43µs |  |  | 15.62µs | 24.21µs | 3 |
| sse-fragmentation › assistant-stream: fragmented SSE events › 1024 KiB, 1 chunks | 63.55µs |  |  | 45.98µs | 63.55µs | 3 |
| sse-fragmentation › assistant-stream: fragmented SSE events › 1024 KiB, 1025 chunks | 234.71µs |  |  | 193.31µs | 344.23µs | 3 |
| thread-scaling › external-store thread: mount+unmount by message count › 10 messages | 4.521ms |  |  | 4.521ms | 6.433ms | 3 |
| thread-scaling › external-store thread: mount+unmount by message count › 100 messages | 29.771ms |  |  | 27.814ms | 40.123ms | 3 |
| thread-scaling › external-store thread: mount+unmount by message count › 1000 messages | 376.753ms |  |  | 320.633ms | 435.602ms | 3 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › 20 message window, 10 messages | 433.23µs |  |  | 407.55µs | 626.18µs | 3 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › 20 message window, 100 messages | 689.47µs |  |  | 642.09µs | 934.98µs | 3 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › 20 message window, 1000 messages | 3.341ms |  |  | 3.138ms | 4.653ms | 3 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › all messages by id, 10 messages | 468.17µs |  |  | 408.27µs | 604.87µs | 3 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › all messages by id, 100 messages | 1.079ms |  |  | 1.079ms | 1.674ms | 3 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › all messages by id, 1000 messages | 10.451ms |  |  | 8.176ms | 15.272ms | 3 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › all messages, 10 messages | 407.43µs |  |  | 345.41µs | 667.45µs | 3 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › all messages, 100 messages | 781.80µs |  |  | 781.80µs | 1.197ms | 3 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › all messages, 1000 messages | 6.239ms |  |  | 5.418ms | 9.906ms | 3 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › provider only, 10 messages | 251.50µs |  |  | 161.45µs | 328.33µs | 3 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › provider only, 100 messages | 400.74µs |  |  | 360.68µs | 536.18µs | 3 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › provider only, 1000 messages | 2.329ms |  |  | 2.329ms | 3.392ms | 3 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › runtime only, 10 messages | 12.60µs |  |  | 11.25µs | 19.92µs | 3 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › runtime only, 100 messages | 26.29µs |  |  | 22.66µs | 34.55µs | 3 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › runtime only, 1000 messages | 195.77µs |  |  | 195.77µs | 306.29µs | 3 |
| thread-scaling › external-store thread: one token changed in the last message, by thread length › 10 messages | 438.77µs |  |  | 392.19µs | 680.34µs | 3 |
| thread-scaling › external-store thread: one token changed in the last message, by thread length › 100 messages | 810.46µs |  |  | 810.46µs | 1.238ms | 3 |
| thread-scaling › external-store thread: one token changed in the last message, by thread length › 1000 messages | 5.887ms |  |  | 5.887ms | 10.929ms | 3 |
| tool-args › assistant-stream: accumulator tool arguments (16-char deltas) › 1000 bytes | 196.90µs |  |  | 162.53µs | 273.57µs | 3 |
| tool-args › assistant-stream: accumulator tool arguments (16-char deltas) › 10000 bytes | 1.779ms |  |  | 1.475ms | 2.358ms | 3 |
| tool-args › assistant-stream: accumulator tool arguments (16-char deltas) › 5000 bytes | 897.39µs |  |  | 748.55µs | 1.191ms | 3 |
| tool-args › assistant-stream: active-reader tool arguments (16-char deltas) › 1000 bytes | 238.02µs |  |  | 181.69µs | 317.41µs | 3 |
| tool-args › assistant-stream: active-reader tool arguments (16-char deltas) › 10000 bytes | 2.099ms |  |  | 1.581ms | 2.684ms | 3 |
| tool-args › assistant-stream: active-reader tool arguments (16-char deltas) › 5000 bytes | 1.059ms |  |  | 800.04µs | 1.366ms | 3 |
| tool-args › assistant-stream: complete accumulated arguments (single delta) › 10,000 array elements | 265.70µs |  |  | 247.01µs | 342.19µs | 3 |
| tool-args › assistant-stream: dense accumulated arguments (16-char deltas) › 2,000 array entries | 20.462ms |  |  | 17.154ms | 25.892ms | 3 |
| tool-args › assistant-stream: dense accumulated arguments (16-char deltas) › 2,000 object entries | 461.969ms |  |  | 461.969ms | 810.818ms | 3 |
| tool-args › assistant-stream: execute-only tool arguments (16-char deltas) › 1000 bytes | 184.46µs |  |  | 130.02µs | 233.49µs | 3 |
| tool-args › assistant-stream: execute-only tool arguments (16-char deltas) › 10000 bytes | 1.544ms |  |  | 1.089ms | 1.901ms | 3 |
| tool-args › assistant-stream: execute-only tool arguments (16-char deltas) › 5000 bytes | 785.99µs |  |  | 542.02µs | 976.37µs | 3 |
| tool-args › assistant-stream: long string arguments (4096-char deltas) › accumulator: 10000 bytes | 162.55µs |  |  | 144.39µs | 203.22µs | 3 |
| tool-args › assistant-stream: long string arguments (4096-char deltas) › accumulator: 50000 bytes | 762.47µs |  |  | 686.60µs | 967.42µs | 3 |
| tool-args › assistant-stream: long string arguments (4096-char deltas) › active-reader: 10000 bytes | 177.67µs |  |  | 155.74µs | 224.65µs | 3 |
| tool-args › assistant-stream: long string arguments (4096-char deltas) › active-reader: 50000 bytes | 792.69µs |  |  | 716.95µs | 1.005ms | 3 |
| tree › tree mount+unmount, 500 leaves x 10 hooks › createTapRoot | 2.622ms |  |  | 2.290ms | 3.714ms | 3 |
| tree › tree mount+unmount, 500 leaves x 10 hooks › createTapRootDeps | 2.670ms |  |  | 2.384ms | 3.717ms | 3 |
| tree › tree mount+unmount, 500 leaves x 10 hooks › createTapRootStable | 2.604ms |  |  | 2.302ms | 3.698ms | 3 |
| tree › tree mount+unmount, 500 leaves x 10 hooks › react | 2.653ms |  |  | 2.166ms | 3.712ms | 3 |
| tree › tree mount+unmount, 500 leaves x 10 hooks › tapRoot | 1.676ms |  |  | 1.520ms | 2.350ms | 3 |
| tree › tree update: one leaf dispatch, 500 leaves x 10 hooks › createTapRoot | 2.492ms |  |  | 2.178ms | 3.512ms | 3 |
| tree › tree update: one leaf dispatch, 500 leaves x 10 hooks › createTapRootDeps | 2.483ms |  |  | 2.213ms | 3.507ms | 3 |
| tree › tree update: one leaf dispatch, 500 leaves x 10 hooks › createTapRootStable | 194.73µs |  |  | 194.73µs | 305.20µs | 3 |
| tree › tree update: one leaf dispatch, 500 leaves x 10 hooks › react | 108.25µs |  |  | 95.17µs | 118.29µs | 3 |
| tree › tree update: one leaf dispatch, 500 leaves x 10 hooks › tapRoot | 1.328ms |  |  | 1.132ms | 1.825ms | 3 |
| useResources › useResources mount+unmount, 500 children x 10 hooks › deps | 1.448ms |  |  | 1.237ms | 2.116ms | 3 |
| useResources › useResources mount+unmount, 500 children x 10 hooks › no-deps | 1.526ms |  |  | 1.331ms | 2.162ms | 3 |
| useResources › useResources: one child dispatch, 500 children x 10 hooks › deps | 37.49µs |  |  | 29.89µs | 47.23µs | 3 |
| useResources › useResources: one child dispatch, 500 children x 10 hooks › no-deps | 39.99µs |  |  | 32.50µs | 49.43µs | 3 |
| useResources › useResources: rebuild elements array, 500 children x 10 hooks › deps | 53.28µs |  |  | 46.72µs | 72.42µs | 3 |
| useResources › useResources: rebuild elements array, 500 children x 10 hooks › no-deps | 1.148ms |  |  | 1.062ms | 1.600ms | 3 |

informational; points come from different runners of the same class, so read trends, not single deltas.
