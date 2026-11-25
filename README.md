## aui-perf nightly record

_7 points · 2026-11-19T04:31:14.259Z to 2026-11-25T04:31:18.143Z · latest runner: Intel(R) Xeon(R) 6975P-C · Node v26.13.0_

| bench | latest | Δ7d | Δ30d | min | max | points |
| --- | ---: | ---: | ---: | ---: | ---: | ---: |
| accumulator › assistant-stream: raw controller enqueue overhead › 10,000 chunks from one source stream | 541.80µs |  |  | 541.80µs | 864.27µs | 7 |
| accumulator › assistant-stream: raw controller enqueue overhead › 10,000 controller.enqueue calls | 767.53µs |  |  | 767.53µs | 1.209ms | 7 |
| accumulator › assistant-stream: same 4000-char text, chunk size A/B › 16 deltas × 250 chars | 36.15µs |  |  | 34.48µs | 58.22µs | 7 |
| accumulator › assistant-stream: same 4000-char text, chunk size A/B › 250 deltas × 16 chars | 372.90µs |  |  | 372.90µs | 666.48µs | 7 |
| accumulator › assistant-stream: same 4000-char text, chunk size A/B › 4000 deltas × 1 char (per-token) | 5.831ms |  |  | 5.831ms | 10.380ms | 7 |
| accumulator › assistant-stream: stream + accumulator per-delta cost (16-char deltas) › 100 deltas | 155.31µs |  |  | 155.31µs | 282.75µs | 7 |
| accumulator › assistant-stream: stream + accumulator per-delta cost (16-char deltas) › 1000 deltas | 1.427ms |  |  | 1.427ms | 2.627ms | 7 |
| accumulator › assistant-stream: stream + accumulator per-delta cost (16-char deltas) › 4000 deltas | 5.729ms |  |  | 5.729ms | 10.360ms | 7 |
| accumulator › assistant-stream: stream round trip baseline, no accumulator › 100 deltas | 6.19µs |  |  | 6.19µs | 10.11µs | 7 |
| accumulator › assistant-stream: stream round trip baseline, no accumulator › 1000 deltas | 52.27µs |  |  | 52.27µs | 85.69µs | 7 |
| accumulator › assistant-stream: stream round trip baseline, no accumulator › 4000 deltas | 208.27µs |  |  | 208.27µs | 340.11µs | 7 |
| ai-sdk-system-metadata › ai-sdk: system-message metadata conversion through the runtime › 128 parts, distinct providers (stress) | 55.87µs |  |  | 54.50µs | 137.06µs | 7 |
| ai-sdk-system-metadata › ai-sdk: system-message metadata conversion through the runtime › 16 parts, one repeated provider | 29.89µs |  |  | 29.89µs | 81.72µs | 7 |
| ai-sdk-system-metadata › ai-sdk: system-message metadata conversion through the runtime › 2 parts, one repeated provider | 31.36µs |  |  | 31.36µs | 83.70µs | 7 |
| ai-sdk-system-metadata › ai-sdk: system-message metadata conversion through the runtime › 512 parts, distinct providers (stress) | 206.95µs |  |  | 198.94µs | 318.13µs | 7 |
| ai-sdk-toolkit › ai-sdk: convert fresh AISDKToolkit schemas › 10 static tools | 44.45µs |  |  | 44.45µs | 77.43µs | 7 |
| ai-sdk-toolkit › ai-sdk: convert fresh AISDKToolkit schemas › 100 static tools | 480.50µs |  |  | 479.31µs | 698.64µs | 7 |
| ai-sdk-toolkit › ai-sdk: reuse converted AISDKToolkit schemas › 10 static tools | 6.09µs |  |  | 6.09µs | 10.45µs | 7 |
| ai-sdk-toolkit › ai-sdk: reuse converted AISDKToolkit schemas › 100 static tools | 51.49µs |  |  | 51.38µs | 83.78µs | 7 |
| data-stream › assistant-stream: data stream decode (16-char deltas) › 100 deltas | 430.55µs |  |  | 430.55µs | 760.16µs | 7 |
| data-stream › assistant-stream: data stream decode (16-char deltas) › 1000 deltas | 3.635ms |  |  | 3.635ms | 6.049ms | 7 |
| data-stream › assistant-stream: data stream decode (16-char deltas) › 4000 deltas | 14.176ms |  |  | 14.176ms | 23.946ms | 7 |
| data-stream › assistant-stream: data stream encode (16-char deltas) › 100 deltas | 203.67µs |  |  | 203.67µs | 359.72µs | 7 |
| data-stream › assistant-stream: data stream encode (16-char deltas) › 1000 deltas | 1.965ms |  |  | 1.965ms | 3.455ms | 7 |
| data-stream › assistant-stream: data stream encode (16-char deltas) › 4000 deltas | 8.032ms |  |  | 8.019ms | 13.626ms | 7 |
| external-message-conversion › core: cached external message conversion, one streaming delta › 1000 messages, 6-part replies | 208.35µs |  |  | 204.94µs | 286.73µs | 7 |
| external-message-conversion › core: cached external message conversion, one streaming delta › 5000 messages, 20-part replies | 1.276ms |  |  | 1.276ms | 2.259ms | 7 |
| external-message-conversion › core: external message reasoning continuations › 100 matches | 41.62µs |  |  | 41.62µs | 69.92µs | 7 |
| external-message-conversion › core: external message reasoning continuations › 1000 matches | 415.52µs |  |  | 415.52µs | 710.18µs | 7 |
| external-message-conversion › core: external message reasoning continuations › 5000 matches | 2.235ms |  |  | 2.235ms | 3.843ms | 7 |
| external-message-conversion › core: external message tool results › 100 matches | 52.57µs |  |  | 52.57µs | 79.69µs | 7 |
| external-message-conversion › core: external message tool results › 1000 matches | 526.93µs |  |  | 526.93µs | 794.72µs | 7 |
| external-message-conversion › core: external message tool results › 5000 matches | 2.771ms |  |  | 2.771ms | 4.273ms | 7 |
| external-message-conversion › core: external message unique tool calls › 100 matches | 27.14µs |  |  | 27.14µs | 42.30µs | 7 |
| external-message-conversion › core: external message unique tool calls › 1000 matches | 253.31µs |  |  | 253.31µs | 416.18µs | 7 |
| external-message-conversion › core: external message unique tool calls › 5000 matches | 1.368ms |  |  | 1.368ms | 2.195ms | 7 |
| from-thread-message-like › core: fromThreadMessageLike text parts › 1 text parts | 0.17µs |  |  | 0.17µs | 0.28µs | 7 |
| from-thread-message-like › core: fromThreadMessageLike text parts › 10 text parts | 0.30µs |  |  | 0.30µs | 0.47µs | 7 |
| from-thread-message-like › core: fromThreadMessageLike text parts › 100 text parts | 1.58µs |  |  | 1.58µs | 2.47µs | 7 |
| from-thread-message-like › core: fromThreadMessageLike tool calls › 1 tool calls | 0.38µs |  |  | 0.38µs | 0.68µs | 7 |
| from-thread-message-like › core: fromThreadMessageLike tool calls › 10 tool calls | 2.23µs |  |  | 2.23µs | 3.51µs | 7 |
| from-thread-message-like › core: fromThreadMessageLike tool calls › 100 tool calls | 20.04µs |  |  | 19.76µs | 31.97µs | 7 |
| interactable-array-patches › core: id-keyed interactable array patches › 1000 items and patches | 112.44µs |  |  | 111.19µs | 150.94µs | 7 |
| interactable-array-patches › core: id-keyed interactable array patches › 5000 items and patches | 640.51µs |  |  | 597.75µs | 847.87µs | 7 |
| markdown-preprocess › react-markdown: preprocess › escapeCurrencyDollars, 20,000 tilde runs on one line | 1.964ms |  |  | 1.951ms | 2.807ms | 7 |
| markdown-preprocess › react-markdown: preprocess › escapeCurrencyDollars, 20,000 tildes after prose | 118.61µs |  |  | 118.35µs | 210.03µs | 7 |
| markdown-preprocess › react-markdown: preprocess › escapeCurrencyDollars, 20,000 triple-backtick spans on one line | 2.524ms |  |  | 2.524ms | 3.711ms | 7 |
| markdown-preprocess › react-markdown: preprocess › escapeCurrencyDollars, 5,000 code spans in one paragraph | 341.56µs |  |  | 336.49µs | 513.75µs | 7 |
| markdown-preprocess › react-markdown: preprocess › escapeCurrencyDollars, mixed message, 100 sections | 506.55µs |  |  | 498.64µs | 709.20µs | 7 |
| markdown-preprocess › react-markdown: preprocess › normalizeMathDelimiters, 20,000 tilde runs on one line | 5.822ms |  |  | 5.643ms | 8.157ms | 7 |
| markdown-preprocess › react-markdown: preprocess › normalizeMathDelimiters, 20,000 tildes after prose | 482.66µs |  |  | 482.66µs | 959.53µs | 7 |
| markdown-preprocess › react-markdown: preprocess › normalizeMathDelimiters, 20,000 triple-backtick spans on one line | 14.666ms |  |  | 14.666ms | 23.972ms | 7 |
| markdown-preprocess › react-markdown: preprocess › normalizeMathDelimiters, 5,000 code spans in one paragraph | 2.308ms |  |  | 2.308ms | 3.956ms | 7 |
| markdown-preprocess › react-markdown: preprocess › normalizeMathDelimiters, mixed message, 100 sections | 1.777ms |  |  | 1.766ms | 2.784ms | 7 |
| markdown-streaming › react-markdown: one token after an unchanged fenced code block › 10 KB fenced Markdown | 1.972ms |  |  | 1.972ms | 3.095ms | 7 |
| markdown-streaming › react-markdown: one token after an unchanged fenced code block › 10 KB fenced Markdown deferred | 2.186ms |  |  | 2.186ms | 3.315ms | 7 |
| markdown-streaming › react-markdown: one token after an unchanged fenced code block › 100 KB fenced Markdown | 13.429ms |  |  | 13.415ms | 20.949ms | 7 |
| markdown-streaming › react-markdown: one token after an unchanged fenced code block › 100 KB fenced Markdown deferred | 14.662ms |  |  | 14.636ms | 22.440ms | 7 |
| markdown-streaming › react-markdown: one token changed in the last paragraph, by message length › 1 paragraphs | 1.106ms |  |  | 1.025ms | 1.555ms | 7 |
| markdown-streaming › react-markdown: one token changed in the last paragraph, by message length › 10 paragraphs | 1.848ms |  |  | 1.848ms | 3.130ms | 7 |
| markdown-streaming › react-markdown: one token changed in the last paragraph, by message length › 50 paragraphs | 6.313ms |  |  | 6.313ms | 10.109ms | 7 |
| markdown-streaming › react-markdown: the same token with defer on › 1 paragraphs deferred | 1.524ms |  |  | 1.171ms | 1.524ms | 7 |
| markdown-streaming › react-markdown: the same token with defer on › 10 paragraphs deferred | 1.395ms |  |  | 1.395ms | 1.928ms | 7 |
| markdown-streaming › react-markdown: the same token with defer on › 50 paragraphs deferred | 3.206ms |  |  | 3.206ms | 4.867ms | 7 |
| react-langgraph › react-langgraph: streamed tool argument accumulation › 1000 character argument in 16-character deltas | 197.04µs |  |  | 194.97µs | 345.80µs | 7 |
| react-langgraph › react-langgraph: streamed tool argument accumulation › 10000 character argument in 16-character deltas | 1.616ms |  |  | 1.616ms | 2.851ms | 7 |
| react-langgraph › react-langgraph: streamed tool argument accumulation › 500 short object entries in 16-character deltas | 181.912ms |  |  | 181.912ms | 312.966ms | 7 |
| react-langgraph › react-langgraph: streamed tool argument accumulation › 50000 character argument in 16-character deltas | 7.867ms |  |  | 7.867ms | 13.543ms | 7 |
| react-pi-message-projection › react-pi: streaming tail projection › 10 stable messages | 1.18µs |  |  | 1.18µs | 2.32µs | 7 |
| react-pi-message-projection › react-pi: streaming tail projection › 1000 stable messages | 5.41µs |  |  | 5.40µs | 10.68µs | 7 |
| react-pi-message-projection › react-pi: streaming tail projection › 5000 stable messages | 25.29µs |  |  | 25.29µs | 48.04µs | 7 |
| sse-fragmentation › assistant-stream: fragmented SSE events › 100 KiB, 1 chunks | 4.70µs |  |  | 4.70µs | 7.33µs | 7 |
| sse-fragmentation › assistant-stream: fragmented SSE events › 100 KiB, 101 chunks | 15.35µs |  |  | 15.35µs | 24.21µs | 7 |
| sse-fragmentation › assistant-stream: fragmented SSE events › 1024 KiB, 1 chunks | 45.83µs |  |  | 45.83µs | 64.46µs | 7 |
| sse-fragmentation › assistant-stream: fragmented SSE events › 1024 KiB, 1025 chunks | 183.03µs |  |  | 183.03µs | 344.23µs | 7 |
| thread-scaling › external-store thread: mount+unmount by message count › 10 messages | 3.941ms |  |  | 3.941ms | 6.950ms | 7 |
| thread-scaling › external-store thread: mount+unmount by message count › 100 messages | 22.883ms |  |  | 22.883ms | 45.070ms | 7 |
| thread-scaling › external-store thread: mount+unmount by message count › 1000 messages | 303.432ms |  |  | 303.432ms | 471.630ms | 7 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › 20 message window, 10 messages | 329.18µs |  |  | 329.18µs | 626.18µs | 7 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › 20 message window, 100 messages | 635.87µs |  |  | 635.87µs | 946.59µs | 7 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › 20 message window, 1000 messages | 2.761ms |  |  | 2.761ms | 4.653ms | 7 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › all messages by id, 10 messages | 336.50µs |  |  | 336.50µs | 635.03µs | 7 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › all messages by id, 100 messages | 1.174ms |  |  | 1.079ms | 1.674ms | 7 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › all messages by id, 1000 messages | 8.034ms |  |  | 8.034ms | 15.272ms | 7 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › all messages, 10 messages | 311.25µs |  |  | 311.25µs | 667.45µs | 7 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › all messages, 100 messages | 864.78µs |  |  | 781.80µs | 1.197ms | 7 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › all messages, 1000 messages | 5.241ms |  |  | 5.241ms | 9.906ms | 7 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › provider only, 10 messages | 145.04µs |  |  | 145.04µs | 333.61µs | 7 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › provider only, 100 messages | 359.63µs |  |  | 359.63µs | 544.61µs | 7 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › provider only, 1000 messages | 2.612ms |  |  | 2.329ms | 3.392ms | 7 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › runtime only, 10 messages | 10.93µs |  |  | 10.93µs | 25.72µs | 7 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › runtime only, 100 messages | 22.08µs |  |  | 22.08µs | 40.73µs | 7 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › runtime only, 1000 messages | 183.75µs |  |  | 183.75µs | 306.29µs | 7 |
| thread-scaling › external-store thread: one token changed in the last message, by thread length › 10 messages | 432.32µs |  |  | 392.19µs | 714.62µs | 7 |
| thread-scaling › external-store thread: one token changed in the last message, by thread length › 100 messages | 871.63µs |  |  | 810.46µs | 1.238ms | 7 |
| thread-scaling › external-store thread: one token changed in the last message, by thread length › 1000 messages | 5.162ms |  |  | 5.162ms | 10.929ms | 7 |
| tool-args › assistant-stream: accumulator tool arguments (16-char deltas) › 1000 bytes | 156.10µs |  |  | 156.10µs | 273.57µs | 7 |
| tool-args › assistant-stream: accumulator tool arguments (16-char deltas) › 10000 bytes | 1.447ms |  |  | 1.447ms | 2.358ms | 7 |
| tool-args › assistant-stream: accumulator tool arguments (16-char deltas) › 5000 bytes | 724.66µs |  |  | 724.66µs | 1.191ms | 7 |
| tool-args › assistant-stream: active-reader tool arguments (16-char deltas) › 1000 bytes | 175.27µs |  |  | 175.27µs | 318.76µs | 7 |
| tool-args › assistant-stream: active-reader tool arguments (16-char deltas) › 10000 bytes | 1.522ms |  |  | 1.522ms | 2.684ms | 7 |
| tool-args › assistant-stream: active-reader tool arguments (16-char deltas) › 5000 bytes | 784.09µs |  |  | 784.09µs | 1.366ms | 7 |
| tool-args › assistant-stream: complete accumulated arguments (single delta) › 10,000 array elements | 245.47µs |  |  | 245.47µs | 346.51µs | 7 |
| tool-args › assistant-stream: dense accumulated arguments (16-char deltas) › 2,000 array entries | 16.472ms |  |  | 16.472ms | 26.611ms | 7 |
| tool-args › assistant-stream: dense accumulated arguments (16-char deltas) › 2,000 object entries | 615.783ms |  |  | 461.969ms | 850.924ms | 7 |
| tool-args › assistant-stream: execute-only tool arguments (16-char deltas) › 1000 bytes | 127.23µs |  |  | 127.23µs | 237.05µs | 7 |
| tool-args › assistant-stream: execute-only tool arguments (16-char deltas) › 10000 bytes | 1.052ms |  |  | 1.052ms | 1.901ms | 7 |
| tool-args › assistant-stream: execute-only tool arguments (16-char deltas) › 5000 bytes | 534.39µs |  |  | 534.39µs | 976.37µs | 7 |
| tool-args › assistant-stream: long string arguments (4096-char deltas) › accumulator: 10000 bytes | 145.52µs |  |  | 144.39µs | 210.61µs | 7 |
| tool-args › assistant-stream: long string arguments (4096-char deltas) › accumulator: 50000 bytes | 718.60µs |  |  | 686.60µs | 980.26µs | 7 |
| tool-args › assistant-stream: long string arguments (4096-char deltas) › active-reader: 10000 bytes | 156.50µs |  |  | 155.74µs | 231.11µs | 7 |
| tool-args › assistant-stream: long string arguments (4096-char deltas) › active-reader: 50000 bytes | 716.23µs |  |  | 716.23µs | 1.020ms | 7 |
| tree › tree mount+unmount, 500 leaves x 10 hooks › createTapRoot | 2.256ms |  |  | 2.256ms | 3.714ms | 7 |
| tree › tree mount+unmount, 500 leaves x 10 hooks › createTapRootDeps | 2.288ms |  |  | 2.288ms | 3.717ms | 7 |
| tree › tree mount+unmount, 500 leaves x 10 hooks › createTapRootStable | 2.221ms |  |  | 2.221ms | 3.698ms | 7 |
| tree › tree mount+unmount, 500 leaves x 10 hooks › react | 2.150ms |  |  | 2.150ms | 3.726ms | 7 |
| tree › tree mount+unmount, 500 leaves x 10 hooks › tapRoot | 1.434ms |  |  | 1.405ms | 2.350ms | 7 |
| tree › tree update: one leaf dispatch, 500 leaves x 10 hooks › createTapRoot | 2.161ms |  |  | 2.161ms | 3.512ms | 7 |
| tree › tree update: one leaf dispatch, 500 leaves x 10 hooks › createTapRootDeps | 2.179ms |  |  | 2.179ms | 3.507ms | 7 |
| tree › tree update: one leaf dispatch, 500 leaves x 10 hooks › createTapRootStable | 166.62µs |  |  | 166.62µs | 305.20µs | 7 |
| tree › tree update: one leaf dispatch, 500 leaves x 10 hooks › react | 95.67µs |  |  | 94.44µs | 148.10µs | 7 |
| tree › tree update: one leaf dispatch, 500 leaves x 10 hooks › tapRoot | 1.108ms |  |  | 1.108ms | 1.825ms | 7 |
| useResources › useResources mount+unmount, 500 children x 10 hooks › deps | 1.185ms |  |  | 1.185ms | 2.116ms | 7 |
| useResources › useResources mount+unmount, 500 children x 10 hooks › no-deps | 1.294ms |  |  | 1.294ms | 2.162ms | 7 |
| useResources › useResources: one child dispatch, 500 children x 10 hooks › deps | 29.71µs |  |  | 29.71µs | 54.18µs | 7 |
| useResources › useResources: one child dispatch, 500 children x 10 hooks › no-deps | 31.55µs |  |  | 31.55µs | 54.70µs | 7 |
| useResources › useResources: rebuild elements array, 500 children x 10 hooks › deps | 45.20µs |  |  | 45.20µs | 72.42µs | 7 |
| useResources › useResources: rebuild elements array, 500 children x 10 hooks › no-deps | 990.30µs |  |  | 990.30µs | 1.600ms | 7 |

informational; points come from different runners of the same class, so read trends, not single deltas.
