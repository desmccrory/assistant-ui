## aui-perf nightly record

_4 points · 2026-11-19T04:31:14.259Z to 2026-11-22T04:30:44.570Z · latest runner: AMD EPYC 7763 64-Core Processor · Node v26.13.0_

| bench | latest | Δ7d | Δ30d | min | max | points |
| --- | ---: | ---: | ---: | ---: | ---: | ---: |
| accumulator › assistant-stream: raw controller enqueue overhead › 10,000 chunks from one source stream | 843.90µs |  |  | 556.28µs | 864.27µs | 4 |
| accumulator › assistant-stream: raw controller enqueue overhead › 10,000 controller.enqueue calls | 1.200ms |  |  | 792.74µs | 1.209ms | 4 |
| accumulator › assistant-stream: same 4000-char text, chunk size A/B › 16 deltas × 250 chars | 55.73µs |  |  | 35.63µs | 58.22µs | 4 |
| accumulator › assistant-stream: same 4000-char text, chunk size A/B › 250 deltas × 16 chars | 636.82µs |  |  | 389.91µs | 666.48µs | 4 |
| accumulator › assistant-stream: same 4000-char text, chunk size A/B › 4000 deltas × 1 char (per-token) | 9.953ms |  |  | 6.020ms | 10.380ms | 4 |
| accumulator › assistant-stream: stream + accumulator per-delta cost (16-char deltas) › 100 deltas | 277.36µs |  |  | 163.68µs | 282.75µs | 4 |
| accumulator › assistant-stream: stream + accumulator per-delta cost (16-char deltas) › 1000 deltas | 2.490ms |  |  | 1.474ms | 2.627ms | 4 |
| accumulator › assistant-stream: stream + accumulator per-delta cost (16-char deltas) › 4000 deltas | 9.788ms |  |  | 5.943ms | 10.360ms | 4 |
| accumulator › assistant-stream: stream round trip baseline, no accumulator › 100 deltas | 9.62µs |  |  | 6.33µs | 10.11µs | 4 |
| accumulator › assistant-stream: stream round trip baseline, no accumulator › 1000 deltas | 85.69µs |  |  | 53.44µs | 85.69µs | 4 |
| accumulator › assistant-stream: stream round trip baseline, no accumulator › 4000 deltas | 340.11µs |  |  | 210.59µs | 340.11µs | 4 |
| ai-sdk-system-metadata › ai-sdk: system-message metadata conversion through the runtime › 128 parts, distinct providers (stress) | 137.06µs |  |  | 54.60µs | 137.06µs | 4 |
| ai-sdk-system-metadata › ai-sdk: system-message metadata conversion through the runtime › 16 parts, one repeated provider | 81.72µs |  |  | 30.52µs | 81.72µs | 4 |
| ai-sdk-system-metadata › ai-sdk: system-message metadata conversion through the runtime › 2 parts, one repeated provider | 83.70µs |  |  | 31.57µs | 83.70µs | 4 |
| ai-sdk-system-metadata › ai-sdk: system-message metadata conversion through the runtime › 512 parts, distinct providers (stress) | 315.43µs |  |  | 200.72µs | 318.13µs | 4 |
| ai-sdk-toolkit › ai-sdk: convert fresh AISDKToolkit schemas › 10 static tools | 73.88µs |  |  | 45.77µs | 77.43µs | 4 |
| ai-sdk-toolkit › ai-sdk: convert fresh AISDKToolkit schemas › 100 static tools | 685.36µs |  |  | 479.31µs | 698.64µs | 4 |
| ai-sdk-toolkit › ai-sdk: reuse converted AISDKToolkit schemas › 10 static tools | 9.88µs |  |  | 6.34µs | 10.45µs | 4 |
| ai-sdk-toolkit › ai-sdk: reuse converted AISDKToolkit schemas › 100 static tools | 83.78µs |  |  | 53.75µs | 83.78µs | 4 |
| data-stream › assistant-stream: data stream decode (16-char deltas) › 100 deltas | 760.16µs |  |  | 440.94µs | 760.16µs | 4 |
| data-stream › assistant-stream: data stream decode (16-char deltas) › 1000 deltas | 6.049ms |  |  | 3.741ms | 6.049ms | 4 |
| data-stream › assistant-stream: data stream decode (16-char deltas) › 4000 deltas | 23.946ms |  |  | 14.585ms | 23.946ms | 4 |
| data-stream › assistant-stream: data stream encode (16-char deltas) › 100 deltas | 351.50µs |  |  | 208.30µs | 359.72µs | 4 |
| data-stream › assistant-stream: data stream encode (16-char deltas) › 1000 deltas | 3.277ms |  |  | 2.025ms | 3.455ms | 4 |
| data-stream › assistant-stream: data stream encode (16-char deltas) › 4000 deltas | 12.969ms |  |  | 8.167ms | 13.626ms | 4 |
| external-message-conversion › core: cached external message conversion, one streaming delta › 1000 messages, 6-part replies | 275.38µs |  |  | 204.94µs | 286.73µs | 4 |
| external-message-conversion › core: cached external message conversion, one streaming delta › 5000 messages, 20-part replies | 1.960ms |  |  | 1.388ms | 2.175ms | 4 |
| external-message-conversion › core: external message reasoning continuations › 100 matches | 68.64µs |  |  | 42.55µs | 69.92µs | 4 |
| external-message-conversion › core: external message reasoning continuations › 1000 matches | 697.06µs |  |  | 431.05µs | 710.18µs | 4 |
| external-message-conversion › core: external message reasoning continuations › 5000 matches | 3.666ms |  |  | 2.327ms | 3.843ms | 4 |
| external-message-conversion › core: external message tool results › 100 matches | 79.69µs |  |  | 53.98µs | 79.69µs | 4 |
| external-message-conversion › core: external message tool results › 1000 matches | 794.72µs |  |  | 546.21µs | 794.72µs | 4 |
| external-message-conversion › core: external message tool results › 5000 matches | 4.177ms |  |  | 2.830ms | 4.273ms | 4 |
| external-message-conversion › core: external message unique tool calls › 100 matches | 42.30µs |  |  | 28.10µs | 42.30µs | 4 |
| external-message-conversion › core: external message unique tool calls › 1000 matches | 416.18µs |  |  | 268.02µs | 416.18µs | 4 |
| external-message-conversion › core: external message unique tool calls › 5000 matches | 2.195ms |  |  | 1.422ms | 2.195ms | 4 |
| from-thread-message-like › core: fromThreadMessageLike text parts › 1 text parts | 0.28µs |  |  | 0.18µs | 0.28µs | 4 |
| from-thread-message-like › core: fromThreadMessageLike text parts › 10 text parts | 0.45µs |  |  | 0.30µs | 0.47µs | 4 |
| from-thread-message-like › core: fromThreadMessageLike text parts › 100 text parts | 2.43µs |  |  | 1.59µs | 2.47µs | 4 |
| from-thread-message-like › core: fromThreadMessageLike tool calls › 1 tool calls | 0.67µs |  |  | 0.38µs | 0.68µs | 4 |
| from-thread-message-like › core: fromThreadMessageLike tool calls › 10 tool calls | 3.49µs |  |  | 2.32µs | 3.51µs | 4 |
| from-thread-message-like › core: fromThreadMessageLike tool calls › 100 tool calls | 31.97µs |  |  | 20.09µs | 31.97µs | 4 |
| interactable-array-patches › core: id-keyed interactable array patches › 1000 items and patches | 143.02µs |  |  | 111.19µs | 150.94µs | 4 |
| interactable-array-patches › core: id-keyed interactable array patches › 5000 items and patches | 799.40µs |  |  | 597.75µs | 847.87µs | 4 |
| markdown-preprocess › react-markdown: preprocess › escapeCurrencyDollars, 20,000 tilde runs on one line | 2.807ms |  |  | 1.951ms | 2.807ms | 4 |
| markdown-preprocess › react-markdown: preprocess › escapeCurrencyDollars, 20,000 tildes after prose | 207.08µs |  |  | 118.35µs | 207.08µs | 4 |
| markdown-preprocess › react-markdown: preprocess › escapeCurrencyDollars, 20,000 triple-backtick spans on one line | 3.711ms |  |  | 2.524ms | 3.711ms | 4 |
| markdown-preprocess › react-markdown: preprocess › escapeCurrencyDollars, 5,000 code spans in one paragraph | 476.10µs |  |  | 336.49µs | 513.75µs | 4 |
| markdown-preprocess › react-markdown: preprocess › escapeCurrencyDollars, mixed message, 100 sections | 709.20µs |  |  | 498.64µs | 709.20µs | 4 |
| markdown-preprocess › react-markdown: preprocess › normalizeMathDelimiters, 20,000 tilde runs on one line | 7.942ms |  |  | 5.643ms | 7.942ms | 4 |
| markdown-preprocess › react-markdown: preprocess › normalizeMathDelimiters, 20,000 tildes after prose | 934.31µs |  |  | 483.83µs | 934.31µs | 4 |
| markdown-preprocess › react-markdown: preprocess › normalizeMathDelimiters, 20,000 triple-backtick spans on one line | 23.972ms |  |  | 14.833ms | 23.972ms | 4 |
| markdown-preprocess › react-markdown: preprocess › normalizeMathDelimiters, 5,000 code spans in one paragraph | 3.715ms |  |  | 2.337ms | 3.956ms | 4 |
| markdown-preprocess › react-markdown: preprocess › normalizeMathDelimiters, mixed message, 100 sections | 2.784ms |  |  | 1.766ms | 2.784ms | 4 |
| markdown-streaming › react-markdown: one token after an unchanged fenced code block › 10 KB fenced Markdown | 3.095ms |  |  | 1.986ms | 3.095ms | 4 |
| markdown-streaming › react-markdown: one token after an unchanged fenced code block › 10 KB fenced Markdown deferred | 3.315ms |  |  | 2.194ms | 3.315ms | 4 |
| markdown-streaming › react-markdown: one token after an unchanged fenced code block › 100 KB fenced Markdown | 20.949ms |  |  | 13.415ms | 20.949ms | 4 |
| markdown-streaming › react-markdown: one token after an unchanged fenced code block › 100 KB fenced Markdown deferred | 22.440ms |  |  | 14.668ms | 22.440ms | 4 |
| markdown-streaming › react-markdown: one token changed in the last paragraph, by message length › 1 paragraphs | 1.555ms |  |  | 1.025ms | 1.555ms | 4 |
| markdown-streaming › react-markdown: one token changed in the last paragraph, by message length › 10 paragraphs | 3.130ms |  |  | 1.946ms | 3.130ms | 4 |
| markdown-streaming › react-markdown: one token changed in the last paragraph, by message length › 50 paragraphs | 9.959ms |  |  | 6.479ms | 10.109ms | 4 |
| markdown-streaming › react-markdown: the same token with defer on › 1 paragraphs deferred | 1.171ms |  |  | 1.171ms | 1.468ms | 4 |
| markdown-streaming › react-markdown: the same token with defer on › 10 paragraphs deferred | 1.902ms |  |  | 1.422ms | 1.928ms | 4 |
| markdown-streaming › react-markdown: the same token with defer on › 50 paragraphs deferred | 4.867ms |  |  | 3.698ms | 4.867ms | 4 |
| react-langgraph › react-langgraph: streamed tool argument accumulation › 1000 character argument in 16-character deltas | 325.37µs |  |  | 194.97µs | 345.80µs | 4 |
| react-langgraph › react-langgraph: streamed tool argument accumulation › 10000 character argument in 16-character deltas | 2.652ms |  |  | 1.670ms | 2.851ms | 4 |
| react-langgraph › react-langgraph: streamed tool argument accumulation › 500 short object entries in 16-character deltas | 299.528ms |  |  | 184.701ms | 312.966ms | 4 |
| react-langgraph › react-langgraph: streamed tool argument accumulation › 50000 character argument in 16-character deltas | 12.557ms |  |  | 8.337ms | 13.543ms | 4 |
| react-pi-message-projection › react-pi: streaming tail projection › 10 stable messages | 2.25µs |  |  | 1.21µs | 2.32µs | 4 |
| react-pi-message-projection › react-pi: streaming tail projection › 1000 stable messages | 9.42µs |  |  | 5.40µs | 10.68µs | 4 |
| react-pi-message-projection › react-pi: streaming tail projection › 5000 stable messages | 40.45µs |  |  | 25.73µs | 48.04µs | 4 |
| sse-fragmentation › assistant-stream: fragmented SSE events › 100 KiB, 1 chunks | 6.43µs |  |  | 4.71µs | 7.33µs | 4 |
| sse-fragmentation › assistant-stream: fragmented SSE events › 100 KiB, 101 chunks | 20.63µs |  |  | 15.62µs | 24.21µs | 4 |
| sse-fragmentation › assistant-stream: fragmented SSE events › 1024 KiB, 1 chunks | 62.77µs |  |  | 45.98µs | 63.55µs | 4 |
| sse-fragmentation › assistant-stream: fragmented SSE events › 1024 KiB, 1025 chunks | 284.91µs |  |  | 193.31µs | 344.23µs | 4 |
| thread-scaling › external-store thread: mount+unmount by message count › 10 messages | 6.950ms |  |  | 4.521ms | 6.950ms | 4 |
| thread-scaling › external-store thread: mount+unmount by message count › 100 messages | 45.070ms |  |  | 27.814ms | 45.070ms | 4 |
| thread-scaling › external-store thread: mount+unmount by message count › 1000 messages | 471.630ms |  |  | 320.633ms | 471.630ms | 4 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › 20 message window, 10 messages | 613.05µs |  |  | 407.55µs | 626.18µs | 4 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › 20 message window, 100 messages | 946.59µs |  |  | 642.09µs | 946.59µs | 4 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › 20 message window, 1000 messages | 4.355ms |  |  | 3.138ms | 4.653ms | 4 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › all messages by id, 10 messages | 635.03µs |  |  | 408.27µs | 635.03µs | 4 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › all messages by id, 100 messages | 1.542ms |  |  | 1.079ms | 1.674ms | 4 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › all messages by id, 1000 messages | 14.064ms |  |  | 8.176ms | 15.272ms | 4 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › all messages, 10 messages | 624.65µs |  |  | 345.41µs | 667.45µs | 4 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › all messages, 100 messages | 1.092ms |  |  | 781.80µs | 1.197ms | 4 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › all messages, 1000 messages | 7.213ms |  |  | 5.418ms | 9.906ms | 4 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › provider only, 10 messages | 333.61µs |  |  | 161.45µs | 333.61µs | 4 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › provider only, 100 messages | 544.61µs |  |  | 360.68µs | 544.61µs | 4 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › provider only, 1000 messages | 3.075ms |  |  | 2.329ms | 3.392ms | 4 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › runtime only, 10 messages | 25.72µs |  |  | 11.25µs | 25.72µs | 4 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › runtime only, 100 messages | 40.73µs |  |  | 22.66µs | 40.73µs | 4 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › runtime only, 1000 messages | 260.42µs |  |  | 195.77µs | 306.29µs | 4 |
| thread-scaling › external-store thread: one token changed in the last message, by thread length › 10 messages | 714.62µs |  |  | 392.19µs | 714.62µs | 4 |
| thread-scaling › external-store thread: one token changed in the last message, by thread length › 100 messages | 1.118ms |  |  | 810.46µs | 1.238ms | 4 |
| thread-scaling › external-store thread: one token changed in the last message, by thread length › 1000 messages | 9.307ms |  |  | 5.887ms | 10.929ms | 4 |
| tool-args › assistant-stream: accumulator tool arguments (16-char deltas) › 1000 bytes | 267.18µs |  |  | 162.53µs | 273.57µs | 4 |
| tool-args › assistant-stream: accumulator tool arguments (16-char deltas) › 10000 bytes | 2.258ms |  |  | 1.475ms | 2.358ms | 4 |
| tool-args › assistant-stream: accumulator tool arguments (16-char deltas) › 5000 bytes | 1.136ms |  |  | 748.55µs | 1.191ms | 4 |
| tool-args › assistant-stream: active-reader tool arguments (16-char deltas) › 1000 bytes | 318.76µs |  |  | 181.69µs | 318.76µs | 4 |
| tool-args › assistant-stream: active-reader tool arguments (16-char deltas) › 10000 bytes | 2.590ms |  |  | 1.581ms | 2.684ms | 4 |
| tool-args › assistant-stream: active-reader tool arguments (16-char deltas) › 5000 bytes | 1.314ms |  |  | 800.04µs | 1.366ms | 4 |
| tool-args › assistant-stream: complete accumulated arguments (single delta) › 10,000 array elements | 346.51µs |  |  | 247.01µs | 346.51µs | 4 |
| tool-args › assistant-stream: dense accumulated arguments (16-char deltas) › 2,000 array entries | 26.611ms |  |  | 17.154ms | 26.611ms | 4 |
| tool-args › assistant-stream: dense accumulated arguments (16-char deltas) › 2,000 object entries | 664.288ms |  |  | 461.969ms | 810.818ms | 4 |
| tool-args › assistant-stream: execute-only tool arguments (16-char deltas) › 1000 bytes | 237.05µs |  |  | 130.02µs | 237.05µs | 4 |
| tool-args › assistant-stream: execute-only tool arguments (16-char deltas) › 10000 bytes | 1.865ms |  |  | 1.089ms | 1.901ms | 4 |
| tool-args › assistant-stream: execute-only tool arguments (16-char deltas) › 5000 bytes | 955.07µs |  |  | 542.02µs | 976.37µs | 4 |
| tool-args › assistant-stream: long string arguments (4096-char deltas) › accumulator: 10000 bytes | 210.61µs |  |  | 144.39µs | 210.61µs | 4 |
| tool-args › assistant-stream: long string arguments (4096-char deltas) › accumulator: 50000 bytes | 980.26µs |  |  | 686.60µs | 980.26µs | 4 |
| tool-args › assistant-stream: long string arguments (4096-char deltas) › active-reader: 10000 bytes | 231.11µs |  |  | 155.74µs | 231.11µs | 4 |
| tool-args › assistant-stream: long string arguments (4096-char deltas) › active-reader: 50000 bytes | 1.020ms |  |  | 716.95µs | 1.020ms | 4 |
| tree › tree mount+unmount, 500 leaves x 10 hooks › createTapRoot | 3.568ms |  |  | 2.290ms | 3.714ms | 4 |
| tree › tree mount+unmount, 500 leaves x 10 hooks › createTapRootDeps | 3.582ms |  |  | 2.384ms | 3.717ms | 4 |
| tree › tree mount+unmount, 500 leaves x 10 hooks › createTapRootStable | 3.525ms |  |  | 2.302ms | 3.698ms | 4 |
| tree › tree mount+unmount, 500 leaves x 10 hooks › react | 3.726ms |  |  | 2.166ms | 3.726ms | 4 |
| tree › tree mount+unmount, 500 leaves x 10 hooks › tapRoot | 2.286ms |  |  | 1.520ms | 2.350ms | 4 |
| tree › tree update: one leaf dispatch, 500 leaves x 10 hooks › createTapRoot | 3.453ms |  |  | 2.178ms | 3.512ms | 4 |
| tree › tree update: one leaf dispatch, 500 leaves x 10 hooks › createTapRootDeps | 3.489ms |  |  | 2.213ms | 3.507ms | 4 |
| tree › tree update: one leaf dispatch, 500 leaves x 10 hooks › createTapRootStable | 248.67µs |  |  | 194.73µs | 305.20µs | 4 |
| tree › tree update: one leaf dispatch, 500 leaves x 10 hooks › react | 148.10µs |  |  | 95.17µs | 148.10µs | 4 |
| tree › tree update: one leaf dispatch, 500 leaves x 10 hooks › tapRoot | 1.752ms |  |  | 1.132ms | 1.825ms | 4 |
| useResources › useResources mount+unmount, 500 children x 10 hooks › deps | 1.979ms |  |  | 1.237ms | 2.116ms | 4 |
| useResources › useResources mount+unmount, 500 children x 10 hooks › no-deps | 2.072ms |  |  | 1.331ms | 2.162ms | 4 |
| useResources › useResources: one child dispatch, 500 children x 10 hooks › deps | 54.18µs |  |  | 29.89µs | 54.18µs | 4 |
| useResources › useResources: one child dispatch, 500 children x 10 hooks › no-deps | 54.70µs |  |  | 32.50µs | 54.70µs | 4 |
| useResources › useResources: rebuild elements array, 500 children x 10 hooks › deps | 70.85µs |  |  | 46.72µs | 72.42µs | 4 |
| useResources › useResources: rebuild elements array, 500 children x 10 hooks › no-deps | 1.526ms |  |  | 1.062ms | 1.600ms | 4 |

informational; points come from different runners of the same class, so read trends, not single deltas.
