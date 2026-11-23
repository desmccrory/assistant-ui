## aui-perf nightly record

_5 points · 2026-11-19T04:31:14.259Z to 2026-11-23T04:33:08.257Z · latest runner: INTEL(R) XEON(R) PLATINUM 8573C · Node v26.13.0_

| bench | latest | Δ7d | Δ30d | min | max | points |
| --- | ---: | ---: | ---: | ---: | ---: | ---: |
| accumulator › assistant-stream: raw controller enqueue overhead › 10,000 chunks from one source stream | 733.41µs |  |  | 556.28µs | 864.27µs | 5 |
| accumulator › assistant-stream: raw controller enqueue overhead › 10,000 controller.enqueue calls | 1.056ms |  |  | 792.74µs | 1.209ms | 5 |
| accumulator › assistant-stream: same 4000-char text, chunk size A/B › 16 deltas × 250 chars | 50.56µs |  |  | 35.63µs | 58.22µs | 5 |
| accumulator › assistant-stream: same 4000-char text, chunk size A/B › 250 deltas × 16 chars | 605.49µs |  |  | 389.91µs | 666.48µs | 5 |
| accumulator › assistant-stream: same 4000-char text, chunk size A/B › 4000 deltas × 1 char (per-token) | 9.621ms |  |  | 6.020ms | 10.380ms | 5 |
| accumulator › assistant-stream: stream + accumulator per-delta cost (16-char deltas) › 100 deltas | 254.16µs |  |  | 163.68µs | 282.75µs | 5 |
| accumulator › assistant-stream: stream + accumulator per-delta cost (16-char deltas) › 1000 deltas | 2.383ms |  |  | 1.474ms | 2.627ms | 5 |
| accumulator › assistant-stream: stream + accumulator per-delta cost (16-char deltas) › 4000 deltas | 9.310ms |  |  | 5.943ms | 10.360ms | 5 |
| accumulator › assistant-stream: stream round trip baseline, no accumulator › 100 deltas | 8.42µs |  |  | 6.33µs | 10.11µs | 5 |
| accumulator › assistant-stream: stream round trip baseline, no accumulator › 1000 deltas | 69.90µs |  |  | 53.44µs | 85.69µs | 5 |
| accumulator › assistant-stream: stream round trip baseline, no accumulator › 4000 deltas | 276.08µs |  |  | 210.59µs | 340.11µs | 5 |
| ai-sdk-system-metadata › ai-sdk: system-message metadata conversion through the runtime › 128 parts, distinct providers (stress) | 83.92µs |  |  | 54.60µs | 137.06µs | 5 |
| ai-sdk-system-metadata › ai-sdk: system-message metadata conversion through the runtime › 16 parts, one repeated provider | 43.44µs |  |  | 30.52µs | 81.72µs | 5 |
| ai-sdk-system-metadata › ai-sdk: system-message metadata conversion through the runtime › 2 parts, one repeated provider | 41.55µs |  |  | 31.57µs | 83.70µs | 5 |
| ai-sdk-system-metadata › ai-sdk: system-message metadata conversion through the runtime › 512 parts, distinct providers (stress) | 303.33µs |  |  | 200.72µs | 318.13µs | 5 |
| ai-sdk-toolkit › ai-sdk: convert fresh AISDKToolkit schemas › 10 static tools | 69.17µs |  |  | 45.77µs | 77.43µs | 5 |
| ai-sdk-toolkit › ai-sdk: convert fresh AISDKToolkit schemas › 100 static tools | 602.63µs |  |  | 479.31µs | 698.64µs | 5 |
| ai-sdk-toolkit › ai-sdk: reuse converted AISDKToolkit schemas › 10 static tools | 9.14µs |  |  | 6.34µs | 10.45µs | 5 |
| ai-sdk-toolkit › ai-sdk: reuse converted AISDKToolkit schemas › 100 static tools | 71.52µs |  |  | 53.75µs | 83.78µs | 5 |
| data-stream › assistant-stream: data stream decode (16-char deltas) › 100 deltas | 622.29µs |  |  | 440.94µs | 760.16µs | 5 |
| data-stream › assistant-stream: data stream decode (16-char deltas) › 1000 deltas | 5.029ms |  |  | 3.741ms | 6.049ms | 5 |
| data-stream › assistant-stream: data stream decode (16-char deltas) › 4000 deltas | 19.336ms |  |  | 14.585ms | 23.946ms | 5 |
| data-stream › assistant-stream: data stream encode (16-char deltas) › 100 deltas | 285.10µs |  |  | 208.30µs | 359.72µs | 5 |
| data-stream › assistant-stream: data stream encode (16-char deltas) › 1000 deltas | 2.895ms |  |  | 2.025ms | 3.455ms | 5 |
| data-stream › assistant-stream: data stream encode (16-char deltas) › 4000 deltas | 11.132ms |  |  | 8.167ms | 13.626ms | 5 |
| external-message-conversion › core: cached external message conversion, one streaming delta › 1000 messages, 6-part replies | 260.39µs |  |  | 204.94µs | 286.73µs | 5 |
| external-message-conversion › core: cached external message conversion, one streaming delta › 5000 messages, 20-part replies | 2.259ms |  |  | 1.388ms | 2.259ms | 5 |
| external-message-conversion › core: external message reasoning continuations › 100 matches | 60.39µs |  |  | 42.55µs | 69.92µs | 5 |
| external-message-conversion › core: external message reasoning continuations › 1000 matches | 601.88µs |  |  | 431.05µs | 710.18µs | 5 |
| external-message-conversion › core: external message reasoning continuations › 5000 matches | 3.108ms |  |  | 2.327ms | 3.843ms | 5 |
| external-message-conversion › core: external message tool results › 100 matches | 70.24µs |  |  | 53.98µs | 79.69µs | 5 |
| external-message-conversion › core: external message tool results › 1000 matches | 706.14µs |  |  | 546.21µs | 794.72µs | 5 |
| external-message-conversion › core: external message tool results › 5000 matches | 3.760ms |  |  | 2.830ms | 4.273ms | 5 |
| external-message-conversion › core: external message unique tool calls › 100 matches | 36.66µs |  |  | 28.10µs | 42.30µs | 5 |
| external-message-conversion › core: external message unique tool calls › 1000 matches | 357.92µs |  |  | 268.02µs | 416.18µs | 5 |
| external-message-conversion › core: external message unique tool calls › 5000 matches | 1.860ms |  |  | 1.422ms | 2.195ms | 5 |
| from-thread-message-like › core: fromThreadMessageLike text parts › 1 text parts | 0.23µs |  |  | 0.18µs | 0.28µs | 5 |
| from-thread-message-like › core: fromThreadMessageLike text parts › 10 text parts | 0.38µs |  |  | 0.30µs | 0.47µs | 5 |
| from-thread-message-like › core: fromThreadMessageLike text parts › 100 text parts | 2.17µs |  |  | 1.59µs | 2.47µs | 5 |
| from-thread-message-like › core: fromThreadMessageLike tool calls › 1 tool calls | 0.53µs |  |  | 0.38µs | 0.68µs | 5 |
| from-thread-message-like › core: fromThreadMessageLike tool calls › 10 tool calls | 2.91µs |  |  | 2.32µs | 3.51µs | 5 |
| from-thread-message-like › core: fromThreadMessageLike tool calls › 100 tool calls | 26.34µs |  |  | 20.09µs | 31.97µs | 5 |
| interactable-array-patches › core: id-keyed interactable array patches › 1000 items and patches | 142.72µs |  |  | 111.19µs | 150.94µs | 5 |
| interactable-array-patches › core: id-keyed interactable array patches › 5000 items and patches | 828.55µs |  |  | 597.75µs | 847.87µs | 5 |
| markdown-preprocess › react-markdown: preprocess › escapeCurrencyDollars, 20,000 tilde runs on one line | 2.772ms |  |  | 1.951ms | 2.807ms | 5 |
| markdown-preprocess › react-markdown: preprocess › escapeCurrencyDollars, 20,000 tildes after prose | 210.03µs |  |  | 118.35µs | 210.03µs | 5 |
| markdown-preprocess › react-markdown: preprocess › escapeCurrencyDollars, 20,000 triple-backtick spans on one line | 3.629ms |  |  | 2.524ms | 3.711ms | 5 |
| markdown-preprocess › react-markdown: preprocess › escapeCurrencyDollars, 5,000 code spans in one paragraph | 448.20µs |  |  | 336.49µs | 513.75µs | 5 |
| markdown-preprocess › react-markdown: preprocess › escapeCurrencyDollars, mixed message, 100 sections | 669.05µs |  |  | 498.64µs | 709.20µs | 5 |
| markdown-preprocess › react-markdown: preprocess › normalizeMathDelimiters, 20,000 tilde runs on one line | 8.157ms |  |  | 5.643ms | 8.157ms | 5 |
| markdown-preprocess › react-markdown: preprocess › normalizeMathDelimiters, 20,000 tildes after prose | 959.53µs |  |  | 483.83µs | 959.53µs | 5 |
| markdown-preprocess › react-markdown: preprocess › normalizeMathDelimiters, 20,000 triple-backtick spans on one line | 19.796ms |  |  | 14.833ms | 23.972ms | 5 |
| markdown-preprocess › react-markdown: preprocess › normalizeMathDelimiters, 5,000 code spans in one paragraph | 3.242ms |  |  | 2.337ms | 3.956ms | 5 |
| markdown-preprocess › react-markdown: preprocess › normalizeMathDelimiters, mixed message, 100 sections | 2.477ms |  |  | 1.766ms | 2.784ms | 5 |
| markdown-streaming › react-markdown: one token after an unchanged fenced code block › 10 KB fenced Markdown | 2.768ms |  |  | 1.986ms | 3.095ms | 5 |
| markdown-streaming › react-markdown: one token after an unchanged fenced code block › 10 KB fenced Markdown deferred | 3.025ms |  |  | 2.194ms | 3.315ms | 5 |
| markdown-streaming › react-markdown: one token after an unchanged fenced code block › 100 KB fenced Markdown | 18.677ms |  |  | 13.415ms | 20.949ms | 5 |
| markdown-streaming › react-markdown: one token after an unchanged fenced code block › 100 KB fenced Markdown deferred | 20.062ms |  |  | 14.668ms | 22.440ms | 5 |
| markdown-streaming › react-markdown: one token changed in the last paragraph, by message length › 1 paragraphs | 1.519ms |  |  | 1.025ms | 1.555ms | 5 |
| markdown-streaming › react-markdown: one token changed in the last paragraph, by message length › 10 paragraphs | 2.911ms |  |  | 1.946ms | 3.130ms | 5 |
| markdown-streaming › react-markdown: one token changed in the last paragraph, by message length › 50 paragraphs | 9.003ms |  |  | 6.479ms | 10.109ms | 5 |
| markdown-streaming › react-markdown: the same token with defer on › 1 paragraphs deferred | 1.247ms |  |  | 1.171ms | 1.468ms | 5 |
| markdown-streaming › react-markdown: the same token with defer on › 10 paragraphs deferred | 1.743ms |  |  | 1.422ms | 1.928ms | 5 |
| markdown-streaming › react-markdown: the same token with defer on › 50 paragraphs deferred | 4.734ms |  |  | 3.698ms | 4.867ms | 5 |
| react-langgraph › react-langgraph: streamed tool argument accumulation › 1000 character argument in 16-character deltas | 310.03µs |  |  | 194.97µs | 345.80µs | 5 |
| react-langgraph › react-langgraph: streamed tool argument accumulation › 10000 character argument in 16-character deltas | 2.525ms |  |  | 1.670ms | 2.851ms | 5 |
| react-langgraph › react-langgraph: streamed tool argument accumulation › 500 short object entries in 16-character deltas | 256.812ms |  |  | 184.701ms | 312.966ms | 5 |
| react-langgraph › react-langgraph: streamed tool argument accumulation › 50000 character argument in 16-character deltas | 12.422ms |  |  | 8.337ms | 13.543ms | 5 |
| react-pi-message-projection › react-pi: streaming tail projection › 10 stable messages | 2.14µs |  |  | 1.21µs | 2.32µs | 5 |
| react-pi-message-projection › react-pi: streaming tail projection › 1000 stable messages | 8.28µs |  |  | 5.40µs | 10.68µs | 5 |
| react-pi-message-projection › react-pi: streaming tail projection › 5000 stable messages | 38.56µs |  |  | 25.73µs | 48.04µs | 5 |
| sse-fragmentation › assistant-stream: fragmented SSE events › 100 KiB, 1 chunks | 6.67µs |  |  | 4.71µs | 7.33µs | 5 |
| sse-fragmentation › assistant-stream: fragmented SSE events › 100 KiB, 101 chunks | 21.71µs |  |  | 15.62µs | 24.21µs | 5 |
| sse-fragmentation › assistant-stream: fragmented SSE events › 1024 KiB, 1 chunks | 64.46µs |  |  | 45.98µs | 64.46µs | 5 |
| sse-fragmentation › assistant-stream: fragmented SSE events › 1024 KiB, 1025 chunks | 220.41µs |  |  | 193.31µs | 344.23µs | 5 |
| thread-scaling › external-store thread: mount+unmount by message count › 10 messages | 5.782ms |  |  | 4.521ms | 6.950ms | 5 |
| thread-scaling › external-store thread: mount+unmount by message count › 100 messages | 35.144ms |  |  | 27.814ms | 45.070ms | 5 |
| thread-scaling › external-store thread: mount+unmount by message count › 1000 messages | 372.913ms |  |  | 320.633ms | 471.630ms | 5 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › 20 message window, 10 messages | 453.38µs |  |  | 407.55µs | 626.18µs | 5 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › 20 message window, 100 messages | 813.62µs |  |  | 642.09µs | 946.59µs | 5 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › 20 message window, 1000 messages | 3.806ms |  |  | 3.138ms | 4.653ms | 5 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › all messages by id, 10 messages | 419.74µs |  |  | 408.27µs | 635.03µs | 5 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › all messages by id, 100 messages | 1.493ms |  |  | 1.079ms | 1.674ms | 5 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › all messages by id, 1000 messages | 10.672ms |  |  | 8.176ms | 15.272ms | 5 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › all messages, 10 messages | 450.93µs |  |  | 345.41µs | 667.45µs | 5 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › all messages, 100 messages | 1.114ms |  |  | 781.80µs | 1.197ms | 5 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › all messages, 1000 messages | 6.908ms |  |  | 5.418ms | 9.906ms | 5 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › provider only, 10 messages | 196.13µs |  |  | 161.45µs | 333.61µs | 5 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › provider only, 100 messages | 446.87µs |  |  | 360.68µs | 544.61µs | 5 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › provider only, 1000 messages | 3.253ms |  |  | 2.329ms | 3.392ms | 5 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › runtime only, 10 messages | 14.79µs |  |  | 11.25µs | 25.72µs | 5 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › runtime only, 100 messages | 29.71µs |  |  | 22.66µs | 40.73µs | 5 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › runtime only, 1000 messages | 260.40µs |  |  | 195.77µs | 306.29µs | 5 |
| thread-scaling › external-store thread: one token changed in the last message, by thread length › 10 messages | 602.69µs |  |  | 392.19µs | 714.62µs | 5 |
| thread-scaling › external-store thread: one token changed in the last message, by thread length › 100 messages | 1.136ms |  |  | 810.46µs | 1.238ms | 5 |
| thread-scaling › external-store thread: one token changed in the last message, by thread length › 1000 messages | 7.014ms |  |  | 5.887ms | 10.929ms | 5 |
| tool-args › assistant-stream: accumulator tool arguments (16-char deltas) › 1000 bytes | 230.25µs |  |  | 162.53µs | 273.57µs | 5 |
| tool-args › assistant-stream: accumulator tool arguments (16-char deltas) › 10000 bytes | 2.081ms |  |  | 1.475ms | 2.358ms | 5 |
| tool-args › assistant-stream: accumulator tool arguments (16-char deltas) › 5000 bytes | 1.043ms |  |  | 748.55µs | 1.191ms | 5 |
| tool-args › assistant-stream: active-reader tool arguments (16-char deltas) › 1000 bytes | 258.61µs |  |  | 181.69µs | 318.76µs | 5 |
| tool-args › assistant-stream: active-reader tool arguments (16-char deltas) › 10000 bytes | 2.286ms |  |  | 1.581ms | 2.684ms | 5 |
| tool-args › assistant-stream: active-reader tool arguments (16-char deltas) › 5000 bytes | 1.163ms |  |  | 800.04µs | 1.366ms | 5 |
| tool-args › assistant-stream: complete accumulated arguments (single delta) › 10,000 array elements | 328.37µs |  |  | 247.01µs | 346.51µs | 5 |
| tool-args › assistant-stream: dense accumulated arguments (16-char deltas) › 2,000 array entries | 21.790ms |  |  | 17.154ms | 26.611ms | 5 |
| tool-args › assistant-stream: dense accumulated arguments (16-char deltas) › 2,000 object entries | 850.924ms |  |  | 461.969ms | 850.924ms | 5 |
| tool-args › assistant-stream: execute-only tool arguments (16-char deltas) › 1000 bytes | 194.10µs |  |  | 130.02µs | 237.05µs | 5 |
| tool-args › assistant-stream: execute-only tool arguments (16-char deltas) › 10000 bytes | 1.570ms |  |  | 1.089ms | 1.901ms | 5 |
| tool-args › assistant-stream: execute-only tool arguments (16-char deltas) › 5000 bytes | 799.21µs |  |  | 542.02µs | 976.37µs | 5 |
| tool-args › assistant-stream: long string arguments (4096-char deltas) › accumulator: 10000 bytes | 190.39µs |  |  | 144.39µs | 210.61µs | 5 |
| tool-args › assistant-stream: long string arguments (4096-char deltas) › accumulator: 50000 bytes | 888.45µs |  |  | 686.60µs | 980.26µs | 5 |
| tool-args › assistant-stream: long string arguments (4096-char deltas) › active-reader: 10000 bytes | 210.81µs |  |  | 155.74µs | 231.11µs | 5 |
| tool-args › assistant-stream: long string arguments (4096-char deltas) › active-reader: 50000 bytes | 927.83µs |  |  | 716.95µs | 1.020ms | 5 |
| tree › tree mount+unmount, 500 leaves x 10 hooks › createTapRoot | 3.190ms |  |  | 2.290ms | 3.714ms | 5 |
| tree › tree mount+unmount, 500 leaves x 10 hooks › createTapRootDeps | 3.101ms |  |  | 2.384ms | 3.717ms | 5 |
| tree › tree mount+unmount, 500 leaves x 10 hooks › createTapRootStable | 3.126ms |  |  | 2.302ms | 3.698ms | 5 |
| tree › tree mount+unmount, 500 leaves x 10 hooks › react | 3.158ms |  |  | 2.166ms | 3.726ms | 5 |
| tree › tree mount+unmount, 500 leaves x 10 hooks › tapRoot | 2.071ms |  |  | 1.520ms | 2.350ms | 5 |
| tree › tree update: one leaf dispatch, 500 leaves x 10 hooks › createTapRoot | 2.944ms |  |  | 2.178ms | 3.512ms | 5 |
| tree › tree update: one leaf dispatch, 500 leaves x 10 hooks › createTapRootDeps | 2.933ms |  |  | 2.213ms | 3.507ms | 5 |
| tree › tree update: one leaf dispatch, 500 leaves x 10 hooks › createTapRootStable | 243.88µs |  |  | 194.73µs | 305.20µs | 5 |
| tree › tree update: one leaf dispatch, 500 leaves x 10 hooks › react | 117.01µs |  |  | 95.17µs | 148.10µs | 5 |
| tree › tree update: one leaf dispatch, 500 leaves x 10 hooks › tapRoot | 1.523ms |  |  | 1.132ms | 1.825ms | 5 |
| useResources › useResources mount+unmount, 500 children x 10 hooks › deps | 1.764ms |  |  | 1.237ms | 2.116ms | 5 |
| useResources › useResources mount+unmount, 500 children x 10 hooks › no-deps | 1.909ms |  |  | 1.331ms | 2.162ms | 5 |
| useResources › useResources: one child dispatch, 500 children x 10 hooks › deps | 43.93µs |  |  | 29.89µs | 54.18µs | 5 |
| useResources › useResources: one child dispatch, 500 children x 10 hooks › no-deps | 44.50µs |  |  | 32.50µs | 54.70µs | 5 |
| useResources › useResources: rebuild elements array, 500 children x 10 hooks › deps | 65.58µs |  |  | 46.72µs | 72.42µs | 5 |
| useResources › useResources: rebuild elements array, 500 children x 10 hooks › no-deps | 1.397ms |  |  | 1.062ms | 1.600ms | 5 |

informational; points come from different runners of the same class, so read trends, not single deltas.
