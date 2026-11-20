## aui-perf nightly record

_2 points · 2026-11-19T04:31:14.259Z to 2026-11-20T04:30:42.408Z · latest runner: Intel(R) Xeon(R) 6975P-C · Node v26.13.0_

| bench | latest | Δ7d | Δ30d | min | max | points |
| --- | ---: | ---: | ---: | ---: | ---: | ---: |
| accumulator › assistant-stream: raw controller enqueue overhead › 10,000 chunks from one source stream | 556.28µs |  |  | 556.28µs | 864.27µs | 2 |
| accumulator › assistant-stream: raw controller enqueue overhead › 10,000 controller.enqueue calls | 792.74µs |  |  | 792.74µs | 1.209ms | 2 |
| accumulator › assistant-stream: same 4000-char text, chunk size A/B › 16 deltas × 250 chars | 35.63µs |  |  | 35.63µs | 58.22µs | 2 |
| accumulator › assistant-stream: same 4000-char text, chunk size A/B › 250 deltas × 16 chars | 389.91µs |  |  | 389.91µs | 666.48µs | 2 |
| accumulator › assistant-stream: same 4000-char text, chunk size A/B › 4000 deltas × 1 char (per-token) | 6.020ms |  |  | 6.020ms | 10.380ms | 2 |
| accumulator › assistant-stream: stream + accumulator per-delta cost (16-char deltas) › 100 deltas | 163.68µs |  |  | 163.68µs | 282.75µs | 2 |
| accumulator › assistant-stream: stream + accumulator per-delta cost (16-char deltas) › 1000 deltas | 1.474ms |  |  | 1.474ms | 2.627ms | 2 |
| accumulator › assistant-stream: stream + accumulator per-delta cost (16-char deltas) › 4000 deltas | 5.943ms |  |  | 5.943ms | 10.360ms | 2 |
| accumulator › assistant-stream: stream round trip baseline, no accumulator › 100 deltas | 6.33µs |  |  | 6.33µs | 10.11µs | 2 |
| accumulator › assistant-stream: stream round trip baseline, no accumulator › 1000 deltas | 53.44µs |  |  | 53.44µs | 83.38µs | 2 |
| accumulator › assistant-stream: stream round trip baseline, no accumulator › 4000 deltas | 210.59µs |  |  | 210.59µs | 327.66µs | 2 |
| ai-sdk-system-metadata › ai-sdk: system-message metadata conversion through the runtime › 128 parts, distinct providers (stress) | 54.60µs |  |  | 54.60µs | 107.40µs | 2 |
| ai-sdk-system-metadata › ai-sdk: system-message metadata conversion through the runtime › 16 parts, one repeated provider | 30.52µs |  |  | 30.52µs | 65.03µs | 2 |
| ai-sdk-system-metadata › ai-sdk: system-message metadata conversion through the runtime › 2 parts, one repeated provider | 31.57µs |  |  | 31.57µs | 63.42µs | 2 |
| ai-sdk-system-metadata › ai-sdk: system-message metadata conversion through the runtime › 512 parts, distinct providers (stress) | 200.72µs |  |  | 200.72µs | 318.13µs | 2 |
| ai-sdk-toolkit › ai-sdk: convert fresh AISDKToolkit schemas › 10 static tools | 45.77µs |  |  | 45.77µs | 77.43µs | 2 |
| ai-sdk-toolkit › ai-sdk: convert fresh AISDKToolkit schemas › 100 static tools | 479.31µs |  |  | 479.31µs | 698.64µs | 2 |
| ai-sdk-toolkit › ai-sdk: reuse converted AISDKToolkit schemas › 10 static tools | 6.34µs |  |  | 6.34µs | 10.45µs | 2 |
| ai-sdk-toolkit › ai-sdk: reuse converted AISDKToolkit schemas › 100 static tools | 53.75µs |  |  | 53.75µs | 82.65µs | 2 |
| data-stream › assistant-stream: data stream decode (16-char deltas) › 100 deltas | 440.94µs |  |  | 440.94µs | 732.11µs | 2 |
| data-stream › assistant-stream: data stream decode (16-char deltas) › 1000 deltas | 3.741ms |  |  | 3.741ms | 5.932ms | 2 |
| data-stream › assistant-stream: data stream decode (16-char deltas) › 4000 deltas | 14.585ms |  |  | 14.585ms | 23.420ms | 2 |
| data-stream › assistant-stream: data stream encode (16-char deltas) › 100 deltas | 208.30µs |  |  | 208.30µs | 359.72µs | 2 |
| data-stream › assistant-stream: data stream encode (16-char deltas) › 1000 deltas | 2.025ms |  |  | 2.025ms | 3.455ms | 2 |
| data-stream › assistant-stream: data stream encode (16-char deltas) › 4000 deltas | 8.167ms |  |  | 8.167ms | 13.626ms | 2 |
| external-message-conversion › core: cached external message conversion, one streaming delta › 1000 messages, 6-part replies | 204.94µs |  |  | 204.94µs | 286.73µs | 2 |
| external-message-conversion › core: cached external message conversion, one streaming delta › 5000 messages, 20-part replies | 1.877ms |  |  | 1.877ms | 2.175ms | 2 |
| external-message-conversion › core: external message reasoning continuations › 100 matches | 42.55µs |  |  | 42.55µs | 69.92µs | 2 |
| external-message-conversion › core: external message reasoning continuations › 1000 matches | 431.05µs |  |  | 431.05µs | 710.18µs | 2 |
| external-message-conversion › core: external message reasoning continuations › 5000 matches | 2.327ms |  |  | 2.327ms | 3.843ms | 2 |
| external-message-conversion › core: external message tool results › 100 matches | 53.98µs |  |  | 53.98µs | 76.59µs | 2 |
| external-message-conversion › core: external message tool results › 1000 matches | 546.21µs |  |  | 546.21µs | 781.90µs | 2 |
| external-message-conversion › core: external message tool results › 5000 matches | 2.830ms |  |  | 2.830ms | 4.273ms | 2 |
| external-message-conversion › core: external message unique tool calls › 100 matches | 28.10µs |  |  | 28.10µs | 40.30µs | 2 |
| external-message-conversion › core: external message unique tool calls › 1000 matches | 268.02µs |  |  | 268.02µs | 396.22µs | 2 |
| external-message-conversion › core: external message unique tool calls › 5000 matches | 1.422ms |  |  | 1.422ms | 2.193ms | 2 |
| from-thread-message-like › core: fromThreadMessageLike text parts › 1 text parts | 0.18µs |  |  | 0.18µs | 0.27µs | 2 |
| from-thread-message-like › core: fromThreadMessageLike text parts › 10 text parts | 0.30µs |  |  | 0.30µs | 0.47µs | 2 |
| from-thread-message-like › core: fromThreadMessageLike text parts › 100 text parts | 1.59µs |  |  | 1.59µs | 2.47µs | 2 |
| from-thread-message-like › core: fromThreadMessageLike tool calls › 1 tool calls | 0.38µs |  |  | 0.38µs | 0.68µs | 2 |
| from-thread-message-like › core: fromThreadMessageLike tool calls › 10 tool calls | 2.32µs |  |  | 2.32µs | 3.51µs | 2 |
| from-thread-message-like › core: fromThreadMessageLike tool calls › 100 tool calls | 20.09µs |  |  | 20.09µs | 30.61µs | 2 |
| interactable-array-patches › core: id-keyed interactable array patches › 1000 items and patches | 114.14µs |  |  | 114.14µs | 150.94µs | 2 |
| interactable-array-patches › core: id-keyed interactable array patches › 5000 items and patches | 632.12µs |  |  | 632.12µs | 847.87µs | 2 |
| markdown-preprocess › react-markdown: preprocess › escapeCurrencyDollars, 20,000 tilde runs on one line | 1.951ms |  |  | 1.951ms | 2.735ms | 2 |
| markdown-preprocess › react-markdown: preprocess › escapeCurrencyDollars, 20,000 tildes after prose | 118.35µs |  |  | 118.35µs | 186.13µs | 2 |
| markdown-preprocess › react-markdown: preprocess › escapeCurrencyDollars, 20,000 triple-backtick spans on one line | 2.524ms |  |  | 2.524ms | 3.695ms | 2 |
| markdown-preprocess › react-markdown: preprocess › escapeCurrencyDollars, 5,000 code spans in one paragraph | 336.49µs |  |  | 336.49µs | 513.75µs | 2 |
| markdown-preprocess › react-markdown: preprocess › escapeCurrencyDollars, mixed message, 100 sections | 498.67µs |  |  | 498.67µs | 695.42µs | 2 |
| markdown-preprocess › react-markdown: preprocess › normalizeMathDelimiters, 20,000 tilde runs on one line | 5.767ms |  |  | 5.767ms | 7.351ms | 2 |
| markdown-preprocess › react-markdown: preprocess › normalizeMathDelimiters, 20,000 tildes after prose | 483.83µs |  |  | 483.83µs | 797.35µs | 2 |
| markdown-preprocess › react-markdown: preprocess › normalizeMathDelimiters, 20,000 triple-backtick spans on one line | 14.833ms |  |  | 14.833ms | 23.646ms | 2 |
| markdown-preprocess › react-markdown: preprocess › normalizeMathDelimiters, 5,000 code spans in one paragraph | 2.337ms |  |  | 2.337ms | 3.956ms | 2 |
| markdown-preprocess › react-markdown: preprocess › normalizeMathDelimiters, mixed message, 100 sections | 1.766ms |  |  | 1.766ms | 2.700ms | 2 |
| markdown-streaming › react-markdown: one token after an unchanged fenced code block › 10 KB fenced Markdown | 1.986ms |  |  | 1.986ms | 2.948ms | 2 |
| markdown-streaming › react-markdown: one token after an unchanged fenced code block › 10 KB fenced Markdown deferred | 2.194ms |  |  | 2.194ms | 3.215ms | 2 |
| markdown-streaming › react-markdown: one token after an unchanged fenced code block › 100 KB fenced Markdown | 13.415ms |  |  | 13.415ms | 20.559ms | 2 |
| markdown-streaming › react-markdown: one token after an unchanged fenced code block › 100 KB fenced Markdown deferred | 14.668ms |  |  | 14.668ms | 21.700ms | 2 |
| markdown-streaming › react-markdown: one token changed in the last paragraph, by message length › 1 paragraphs | 1.138ms |  |  | 1.138ms | 1.466ms | 2 |
| markdown-streaming › react-markdown: one token changed in the last paragraph, by message length › 10 paragraphs | 1.946ms |  |  | 1.946ms | 3.042ms | 2 |
| markdown-streaming › react-markdown: one token changed in the last paragraph, by message length › 50 paragraphs | 6.479ms |  |  | 6.479ms | 10.109ms | 2 |
| markdown-streaming › react-markdown: the same token with defer on › 1 paragraphs deferred | 1.447ms |  |  | 1.187ms | 1.447ms | 2 |
| markdown-streaming › react-markdown: the same token with defer on › 10 paragraphs deferred | 1.461ms |  |  | 1.461ms | 1.928ms | 2 |
| markdown-streaming › react-markdown: the same token with defer on › 50 paragraphs deferred | 3.698ms |  |  | 3.698ms | 4.642ms | 2 |
| react-langgraph › react-langgraph: streamed tool argument accumulation › 1000 character argument in 16-character deltas | 194.97µs |  |  | 194.97µs | 345.80µs | 2 |
| react-langgraph › react-langgraph: streamed tool argument accumulation › 10000 character argument in 16-character deltas | 1.670ms |  |  | 1.670ms | 2.851ms | 2 |
| react-langgraph › react-langgraph: streamed tool argument accumulation › 500 short object entries in 16-character deltas | 184.701ms |  |  | 184.701ms | 312.966ms | 2 |
| react-langgraph › react-langgraph: streamed tool argument accumulation › 50000 character argument in 16-character deltas | 8.337ms |  |  | 8.337ms | 13.543ms | 2 |
| react-pi-message-projection › react-pi: streaming tail projection › 10 stable messages | 1.21µs |  |  | 1.21µs | 2.32µs | 2 |
| react-pi-message-projection › react-pi: streaming tail projection › 1000 stable messages | 5.40µs |  |  | 5.40µs | 10.68µs | 2 |
| react-pi-message-projection › react-pi: streaming tail projection › 5000 stable messages | 25.73µs |  |  | 25.73µs | 48.04µs | 2 |
| sse-fragmentation › assistant-stream: fragmented SSE events › 100 KiB, 1 chunks | 4.71µs |  |  | 4.71µs | 5.99µs | 2 |
| sse-fragmentation › assistant-stream: fragmented SSE events › 100 KiB, 101 chunks | 15.62µs |  |  | 15.62µs | 24.21µs | 2 |
| sse-fragmentation › assistant-stream: fragmented SSE events › 1024 KiB, 1 chunks | 45.98µs |  |  | 45.98µs | 57.82µs | 2 |
| sse-fragmentation › assistant-stream: fragmented SSE events › 1024 KiB, 1025 chunks | 193.31µs |  |  | 193.31µs | 344.23µs | 2 |
| thread-scaling › external-store thread: mount+unmount by message count › 10 messages | 4.571ms |  |  | 4.571ms | 6.433ms | 2 |
| thread-scaling › external-store thread: mount+unmount by message count › 100 messages | 27.814ms |  |  | 27.814ms | 40.123ms | 2 |
| thread-scaling › external-store thread: mount+unmount by message count › 1000 messages | 320.633ms |  |  | 320.633ms | 435.602ms | 2 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › 20 message window, 10 messages | 407.55µs |  |  | 407.55µs | 626.18µs | 2 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › 20 message window, 100 messages | 642.09µs |  |  | 642.09µs | 934.98µs | 2 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › 20 message window, 1000 messages | 3.138ms |  |  | 3.138ms | 4.653ms | 2 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › all messages by id, 10 messages | 408.27µs |  |  | 408.27µs | 604.87µs | 2 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › all messages by id, 100 messages | 1.120ms |  |  | 1.120ms | 1.674ms | 2 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › all messages by id, 1000 messages | 8.176ms |  |  | 8.176ms | 15.272ms | 2 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › all messages, 10 messages | 345.41µs |  |  | 345.41µs | 667.45µs | 2 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › all messages, 100 messages | 840.56µs |  |  | 840.56µs | 1.197ms | 2 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › all messages, 1000 messages | 5.418ms |  |  | 5.418ms | 9.906ms | 2 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › provider only, 10 messages | 161.45µs |  |  | 161.45µs | 328.33µs | 2 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › provider only, 100 messages | 360.68µs |  |  | 360.68µs | 536.18µs | 2 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › provider only, 1000 messages | 2.666ms |  |  | 2.666ms | 3.392ms | 2 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › runtime only, 10 messages | 11.25µs |  |  | 11.25µs | 19.92µs | 2 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › runtime only, 100 messages | 22.66µs |  |  | 22.66µs | 34.55µs | 2 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › runtime only, 1000 messages | 196.69µs |  |  | 196.69µs | 306.29µs | 2 |
| thread-scaling › external-store thread: one token changed in the last message, by thread length › 10 messages | 392.19µs |  |  | 392.19µs | 680.34µs | 2 |
| thread-scaling › external-store thread: one token changed in the last message, by thread length › 100 messages | 855.12µs |  |  | 855.12µs | 1.238ms | 2 |
| thread-scaling › external-store thread: one token changed in the last message, by thread length › 1000 messages | 6.029ms |  |  | 6.029ms | 10.929ms | 2 |
| tool-args › assistant-stream: accumulator tool arguments (16-char deltas) › 1000 bytes | 162.53µs |  |  | 162.53µs | 273.57µs | 2 |
| tool-args › assistant-stream: accumulator tool arguments (16-char deltas) › 10000 bytes | 1.475ms |  |  | 1.475ms | 2.358ms | 2 |
| tool-args › assistant-stream: accumulator tool arguments (16-char deltas) › 5000 bytes | 748.55µs |  |  | 748.55µs | 1.191ms | 2 |
| tool-args › assistant-stream: active-reader tool arguments (16-char deltas) › 1000 bytes | 181.69µs |  |  | 181.69µs | 317.41µs | 2 |
| tool-args › assistant-stream: active-reader tool arguments (16-char deltas) › 10000 bytes | 1.581ms |  |  | 1.581ms | 2.684ms | 2 |
| tool-args › assistant-stream: active-reader tool arguments (16-char deltas) › 5000 bytes | 800.04µs |  |  | 800.04µs | 1.366ms | 2 |
| tool-args › assistant-stream: complete accumulated arguments (single delta) › 10,000 array elements | 247.01µs |  |  | 247.01µs | 342.19µs | 2 |
| tool-args › assistant-stream: dense accumulated arguments (16-char deltas) › 2,000 array entries | 17.154ms |  |  | 17.154ms | 25.892ms | 2 |
| tool-args › assistant-stream: dense accumulated arguments (16-char deltas) › 2,000 object entries | 665.928ms |  |  | 665.928ms | 810.818ms | 2 |
| tool-args › assistant-stream: execute-only tool arguments (16-char deltas) › 1000 bytes | 130.02µs |  |  | 130.02µs | 233.49µs | 2 |
| tool-args › assistant-stream: execute-only tool arguments (16-char deltas) › 10000 bytes | 1.089ms |  |  | 1.089ms | 1.901ms | 2 |
| tool-args › assistant-stream: execute-only tool arguments (16-char deltas) › 5000 bytes | 542.02µs |  |  | 542.02µs | 976.37µs | 2 |
| tool-args › assistant-stream: long string arguments (4096-char deltas) › accumulator: 10000 bytes | 144.39µs |  |  | 144.39µs | 203.22µs | 2 |
| tool-args › assistant-stream: long string arguments (4096-char deltas) › accumulator: 50000 bytes | 686.60µs |  |  | 686.60µs | 967.42µs | 2 |
| tool-args › assistant-stream: long string arguments (4096-char deltas) › active-reader: 10000 bytes | 155.74µs |  |  | 155.74µs | 224.65µs | 2 |
| tool-args › assistant-stream: long string arguments (4096-char deltas) › active-reader: 50000 bytes | 716.95µs |  |  | 716.95µs | 1.005ms | 2 |
| tree › tree mount+unmount, 500 leaves x 10 hooks › createTapRoot | 2.290ms |  |  | 2.290ms | 3.714ms | 2 |
| tree › tree mount+unmount, 500 leaves x 10 hooks › createTapRootDeps | 2.384ms |  |  | 2.384ms | 3.717ms | 2 |
| tree › tree mount+unmount, 500 leaves x 10 hooks › createTapRootStable | 2.302ms |  |  | 2.302ms | 3.698ms | 2 |
| tree › tree mount+unmount, 500 leaves x 10 hooks › react | 2.166ms |  |  | 2.166ms | 3.712ms | 2 |
| tree › tree mount+unmount, 500 leaves x 10 hooks › tapRoot | 1.520ms |  |  | 1.520ms | 2.350ms | 2 |
| tree › tree update: one leaf dispatch, 500 leaves x 10 hooks › createTapRoot | 2.178ms |  |  | 2.178ms | 3.512ms | 2 |
| tree › tree update: one leaf dispatch, 500 leaves x 10 hooks › createTapRootDeps | 2.213ms |  |  | 2.213ms | 3.507ms | 2 |
| tree › tree update: one leaf dispatch, 500 leaves x 10 hooks › createTapRootStable | 220.69µs |  |  | 220.69µs | 305.20µs | 2 |
| tree › tree update: one leaf dispatch, 500 leaves x 10 hooks › react | 95.17µs |  |  | 95.17µs | 118.29µs | 2 |
| tree › tree update: one leaf dispatch, 500 leaves x 10 hooks › tapRoot | 1.132ms |  |  | 1.132ms | 1.825ms | 2 |
| useResources › useResources mount+unmount, 500 children x 10 hooks › deps | 1.237ms |  |  | 1.237ms | 2.116ms | 2 |
| useResources › useResources mount+unmount, 500 children x 10 hooks › no-deps | 1.331ms |  |  | 1.331ms | 2.162ms | 2 |
| useResources › useResources: one child dispatch, 500 children x 10 hooks › deps | 29.89µs |  |  | 29.89µs | 47.23µs | 2 |
| useResources › useResources: one child dispatch, 500 children x 10 hooks › no-deps | 32.50µs |  |  | 32.50µs | 49.43µs | 2 |
| useResources › useResources: rebuild elements array, 500 children x 10 hooks › deps | 46.72µs |  |  | 46.72µs | 72.42µs | 2 |
| useResources › useResources: rebuild elements array, 500 children x 10 hooks › no-deps | 1.062ms |  |  | 1.062ms | 1.600ms | 2 |

informational; points come from different runners of the same class, so read trends, not single deltas.
