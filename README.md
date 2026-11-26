## aui-perf nightly record

_8 points · 2026-11-19T04:31:14.259Z to 2026-11-26T04:30:41.179Z · latest runner: AMD EPYC 9V74 80-Core Processor · Node v26.13.0_

| bench | latest | Δ7d | Δ30d | min | max | points |
| --- | ---: | ---: | ---: | ---: | ---: | ---: |
| accumulator › assistant-stream: raw controller enqueue overhead › 10,000 chunks from one source stream | 673.34µs |  |  | 541.80µs | 864.27µs | 8 |
| accumulator › assistant-stream: raw controller enqueue overhead › 10,000 controller.enqueue calls | 1.004ms |  |  | 767.53µs | 1.209ms | 8 |
| accumulator › assistant-stream: same 4000-char text, chunk size A/B › 16 deltas × 250 chars | 46.09µs |  |  | 34.48µs | 58.22µs | 8 |
| accumulator › assistant-stream: same 4000-char text, chunk size A/B › 250 deltas × 16 chars | 531.79µs |  |  | 372.90µs | 666.48µs | 8 |
| accumulator › assistant-stream: same 4000-char text, chunk size A/B › 4000 deltas × 1 char (per-token) | 8.229ms |  |  | 5.831ms | 10.380ms | 8 |
| accumulator › assistant-stream: stream + accumulator per-delta cost (16-char deltas) › 100 deltas | 222.20µs |  |  | 155.31µs | 282.75µs | 8 |
| accumulator › assistant-stream: stream + accumulator per-delta cost (16-char deltas) › 1000 deltas | 2.063ms |  |  | 1.427ms | 2.627ms | 8 |
| accumulator › assistant-stream: stream + accumulator per-delta cost (16-char deltas) › 4000 deltas | 8.205ms |  |  | 5.729ms | 10.360ms | 8 |
| accumulator › assistant-stream: stream round trip baseline, no accumulator › 100 deltas | 8.16µs |  |  | 6.19µs | 10.11µs | 8 |
| accumulator › assistant-stream: stream round trip baseline, no accumulator › 1000 deltas | 68.01µs |  |  | 52.27µs | 85.69µs | 8 |
| accumulator › assistant-stream: stream round trip baseline, no accumulator › 4000 deltas | 265.98µs |  |  | 208.27µs | 340.11µs | 8 |
| ai-sdk-system-metadata › ai-sdk: system-message metadata conversion through the runtime › 128 parts, distinct providers (stress) | 83.44µs |  |  | 54.50µs | 137.06µs | 8 |
| ai-sdk-system-metadata › ai-sdk: system-message metadata conversion through the runtime › 16 parts, one repeated provider | 44.49µs |  |  | 29.89µs | 81.72µs | 8 |
| ai-sdk-system-metadata › ai-sdk: system-message metadata conversion through the runtime › 2 parts, one repeated provider | 42.59µs |  |  | 31.36µs | 83.70µs | 8 |
| ai-sdk-system-metadata › ai-sdk: system-message metadata conversion through the runtime › 512 parts, distinct providers (stress) | 266.30µs |  |  | 198.94µs | 318.13µs | 8 |
| ai-sdk-toolkit › ai-sdk: convert fresh AISDKToolkit schemas › 10 static tools | 54.84µs |  |  | 44.45µs | 77.43µs | 8 |
| ai-sdk-toolkit › ai-sdk: convert fresh AISDKToolkit schemas › 100 static tools | 550.12µs |  |  | 479.31µs | 698.64µs | 8 |
| ai-sdk-toolkit › ai-sdk: reuse converted AISDKToolkit schemas › 10 static tools | 7.69µs |  |  | 6.09µs | 10.45µs | 8 |
| ai-sdk-toolkit › ai-sdk: reuse converted AISDKToolkit schemas › 100 static tools | 62.90µs |  |  | 51.38µs | 83.78µs | 8 |
| data-stream › assistant-stream: data stream decode (16-char deltas) › 100 deltas | 602.75µs |  |  | 430.55µs | 760.16µs | 8 |
| data-stream › assistant-stream: data stream decode (16-char deltas) › 1000 deltas | 5.116ms |  |  | 3.635ms | 6.049ms | 8 |
| data-stream › assistant-stream: data stream decode (16-char deltas) › 4000 deltas | 20.215ms |  |  | 14.176ms | 23.946ms | 8 |
| data-stream › assistant-stream: data stream encode (16-char deltas) › 100 deltas | 293.10µs |  |  | 203.67µs | 359.72µs | 8 |
| data-stream › assistant-stream: data stream encode (16-char deltas) › 1000 deltas | 2.939ms |  |  | 1.965ms | 3.455ms | 8 |
| data-stream › assistant-stream: data stream encode (16-char deltas) › 4000 deltas | 11.840ms |  |  | 8.019ms | 13.626ms | 8 |
| external-message-conversion › core: cached external message conversion, one streaming delta › 1000 messages, 6-part replies | 217.51µs |  |  | 204.94µs | 286.73µs | 8 |
| external-message-conversion › core: cached external message conversion, one streaming delta › 5000 messages, 20-part replies | 1.463ms |  |  | 1.276ms | 2.259ms | 8 |
| external-message-conversion › core: external message reasoning continuations › 100 matches | 50.64µs |  |  | 41.62µs | 69.92µs | 8 |
| external-message-conversion › core: external message reasoning continuations › 1000 matches | 508.86µs |  |  | 415.52µs | 710.18µs | 8 |
| external-message-conversion › core: external message reasoning continuations › 5000 matches | 2.722ms |  |  | 2.235ms | 3.843ms | 8 |
| external-message-conversion › core: external message tool results › 100 matches | 58.91µs |  |  | 52.57µs | 79.69µs | 8 |
| external-message-conversion › core: external message tool results › 1000 matches | 599.41µs |  |  | 526.93µs | 794.72µs | 8 |
| external-message-conversion › core: external message tool results › 5000 matches | 3.126ms |  |  | 2.771ms | 4.273ms | 8 |
| external-message-conversion › core: external message unique tool calls › 100 matches | 31.49µs |  |  | 27.14µs | 42.30µs | 8 |
| external-message-conversion › core: external message unique tool calls › 1000 matches | 300.95µs |  |  | 253.31µs | 416.18µs | 8 |
| external-message-conversion › core: external message unique tool calls › 5000 matches | 1.590ms |  |  | 1.368ms | 2.195ms | 8 |
| from-thread-message-like › core: fromThreadMessageLike text parts › 1 text parts | 0.22µs |  |  | 0.17µs | 0.28µs | 8 |
| from-thread-message-like › core: fromThreadMessageLike text parts › 10 text parts | 0.37µs |  |  | 0.30µs | 0.47µs | 8 |
| from-thread-message-like › core: fromThreadMessageLike text parts › 100 text parts | 2.18µs |  |  | 1.58µs | 2.47µs | 8 |
| from-thread-message-like › core: fromThreadMessageLike tool calls › 1 tool calls | 0.50µs |  |  | 0.38µs | 0.68µs | 8 |
| from-thread-message-like › core: fromThreadMessageLike tool calls › 10 tool calls | 2.57µs |  |  | 2.23µs | 3.51µs | 8 |
| from-thread-message-like › core: fromThreadMessageLike tool calls › 100 tool calls | 24.02µs |  |  | 19.76µs | 31.97µs | 8 |
| interactable-array-patches › core: id-keyed interactable array patches › 1000 items and patches | 117.93µs |  |  | 111.19µs | 150.94µs | 8 |
| interactable-array-patches › core: id-keyed interactable array patches › 5000 items and patches | 618.55µs |  |  | 597.75µs | 847.87µs | 8 |
| markdown-preprocess › react-markdown: preprocess › escapeCurrencyDollars, 20,000 tilde runs on one line | 2.127ms |  |  | 1.951ms | 2.807ms | 8 |
| markdown-preprocess › react-markdown: preprocess › escapeCurrencyDollars, 20,000 tildes after prose | 160.97µs |  |  | 118.35µs | 210.03µs | 8 |
| markdown-preprocess › react-markdown: preprocess › escapeCurrencyDollars, 20,000 triple-backtick spans on one line | 2.758ms |  |  | 2.524ms | 3.711ms | 8 |
| markdown-preprocess › react-markdown: preprocess › escapeCurrencyDollars, 5,000 code spans in one paragraph | 392.73µs |  |  | 336.49µs | 513.75µs | 8 |
| markdown-preprocess › react-markdown: preprocess › escapeCurrencyDollars, mixed message, 100 sections | 501.73µs |  |  | 498.64µs | 709.20µs | 8 |
| markdown-preprocess › react-markdown: preprocess › normalizeMathDelimiters, 20,000 tilde runs on one line | 6.109ms |  |  | 5.643ms | 8.157ms | 8 |
| markdown-preprocess › react-markdown: preprocess › normalizeMathDelimiters, 20,000 tildes after prose | 743.24µs |  |  | 482.66µs | 959.53µs | 8 |
| markdown-preprocess › react-markdown: preprocess › normalizeMathDelimiters, 20,000 triple-backtick spans on one line | 16.784ms |  |  | 14.666ms | 23.972ms | 8 |
| markdown-preprocess › react-markdown: preprocess › normalizeMathDelimiters, 5,000 code spans in one paragraph | 2.758ms |  |  | 2.308ms | 3.956ms | 8 |
| markdown-preprocess › react-markdown: preprocess › normalizeMathDelimiters, mixed message, 100 sections | 1.936ms |  |  | 1.766ms | 2.784ms | 8 |
| markdown-streaming › react-markdown: one token after an unchanged fenced code block › 10 KB fenced Markdown | 2.338ms |  |  | 1.972ms | 3.095ms | 8 |
| markdown-streaming › react-markdown: one token after an unchanged fenced code block › 10 KB fenced Markdown deferred | 2.482ms |  |  | 2.186ms | 3.315ms | 8 |
| markdown-streaming › react-markdown: one token after an unchanged fenced code block › 100 KB fenced Markdown | 16.929ms |  |  | 13.415ms | 20.949ms | 8 |
| markdown-streaming › react-markdown: one token after an unchanged fenced code block › 100 KB fenced Markdown deferred | 18.377ms |  |  | 14.636ms | 22.440ms | 8 |
| markdown-streaming › react-markdown: one token changed in the last paragraph, by message length › 1 paragraphs | 1.039ms |  |  | 1.025ms | 1.555ms | 8 |
| markdown-streaming › react-markdown: one token changed in the last paragraph, by message length › 10 paragraphs | 2.171ms |  |  | 1.848ms | 3.130ms | 8 |
| markdown-streaming › react-markdown: one token changed in the last paragraph, by message length › 50 paragraphs | 7.597ms |  |  | 6.313ms | 10.109ms | 8 |
| markdown-streaming › react-markdown: the same token with defer on › 1 paragraphs deferred | 1.345ms |  |  | 1.171ms | 1.524ms | 8 |
| markdown-streaming › react-markdown: the same token with defer on › 10 paragraphs deferred | 1.455ms |  |  | 1.395ms | 1.928ms | 8 |
| markdown-streaming › react-markdown: the same token with defer on › 50 paragraphs deferred | 4.360ms |  |  | 3.206ms | 4.867ms | 8 |
| react-langgraph › react-langgraph: streamed tool argument accumulation › 1000 character argument in 16-character deltas | 261.59µs |  |  | 194.97µs | 345.80µs | 8 |
| react-langgraph › react-langgraph: streamed tool argument accumulation › 10000 character argument in 16-character deltas | 2.189ms |  |  | 1.616ms | 2.851ms | 8 |
| react-langgraph › react-langgraph: streamed tool argument accumulation › 500 short object entries in 16-character deltas | 221.509ms |  |  | 181.912ms | 312.966ms | 8 |
| react-langgraph › react-langgraph: streamed tool argument accumulation › 50000 character argument in 16-character deltas | 10.919ms |  |  | 7.867ms | 13.543ms | 8 |
| react-pi-message-projection › react-pi: streaming tail projection › 10 stable messages | 1.90µs |  |  | 1.18µs | 2.32µs | 8 |
| react-pi-message-projection › react-pi: streaming tail projection › 1000 stable messages | 9.82µs |  |  | 5.40µs | 10.68µs | 8 |
| react-pi-message-projection › react-pi: streaming tail projection › 5000 stable messages | 40.07µs |  |  | 25.29µs | 48.04µs | 8 |
| sse-fragmentation › assistant-stream: fragmented SSE events › 100 KiB, 1 chunks | 7.35µs |  |  | 4.70µs | 7.35µs | 8 |
| sse-fragmentation › assistant-stream: fragmented SSE events › 100 KiB, 101 chunks | 22.02µs |  |  | 15.35µs | 24.21µs | 8 |
| sse-fragmentation › assistant-stream: fragmented SSE events › 1024 KiB, 1 chunks | 72.66µs |  |  | 45.83µs | 72.66µs | 8 |
| sse-fragmentation › assistant-stream: fragmented SSE events › 1024 KiB, 1025 chunks | 243.55µs |  |  | 183.03µs | 344.23µs | 8 |
| thread-scaling › external-store thread: mount+unmount by message count › 10 messages | 4.816ms |  |  | 3.941ms | 6.950ms | 8 |
| thread-scaling › external-store thread: mount+unmount by message count › 100 messages | 34.399ms |  |  | 22.883ms | 45.070ms | 8 |
| thread-scaling › external-store thread: mount+unmount by message count › 1000 messages | 401.201ms |  |  | 303.432ms | 471.630ms | 8 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › 20 message window, 10 messages | 497.68µs |  |  | 329.18µs | 626.18µs | 8 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › 20 message window, 100 messages | 756.55µs |  |  | 635.87µs | 946.59µs | 8 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › 20 message window, 1000 messages | 3.218ms |  |  | 2.761ms | 4.653ms | 8 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › all messages by id, 10 messages | 481.29µs |  |  | 336.50µs | 635.03µs | 8 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › all messages by id, 100 messages | 1.193ms |  |  | 1.079ms | 1.674ms | 8 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › all messages by id, 1000 messages | 13.808ms |  |  | 8.034ms | 15.272ms | 8 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › all messages, 10 messages | 480.05µs |  |  | 311.25µs | 667.45µs | 8 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › all messages, 100 messages | 845.35µs |  |  | 781.80µs | 1.197ms | 8 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › all messages, 1000 messages | 8.849ms |  |  | 5.241ms | 9.906ms | 8 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › provider only, 10 messages | 270.63µs |  |  | 145.04µs | 333.61µs | 8 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › provider only, 100 messages | 460.12µs |  |  | 359.63µs | 544.61µs | 8 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › provider only, 1000 messages | 2.869ms |  |  | 2.329ms | 3.392ms | 8 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › runtime only, 10 messages | 14.03µs |  |  | 10.93µs | 25.72µs | 8 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › runtime only, 100 messages | 27.54µs |  |  | 22.08µs | 40.73µs | 8 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › runtime only, 1000 messages | 202.95µs |  |  | 183.75µs | 306.29µs | 8 |
| thread-scaling › external-store thread: one token changed in the last message, by thread length › 10 messages | 452.68µs |  |  | 392.19µs | 714.62µs | 8 |
| thread-scaling › external-store thread: one token changed in the last message, by thread length › 100 messages | 842.10µs |  |  | 810.46µs | 1.238ms | 8 |
| thread-scaling › external-store thread: one token changed in the last message, by thread length › 1000 messages | 8.818ms |  |  | 5.162ms | 10.929ms | 8 |
| tool-args › assistant-stream: accumulator tool arguments (16-char deltas) › 1000 bytes | 203.75µs |  |  | 156.10µs | 273.57µs | 8 |
| tool-args › assistant-stream: accumulator tool arguments (16-char deltas) › 10000 bytes | 1.804ms |  |  | 1.447ms | 2.358ms | 8 |
| tool-args › assistant-stream: accumulator tool arguments (16-char deltas) › 5000 bytes | 913.24µs |  |  | 724.66µs | 1.191ms | 8 |
| tool-args › assistant-stream: active-reader tool arguments (16-char deltas) › 1000 bytes | 245.70µs |  |  | 175.27µs | 318.76µs | 8 |
| tool-args › assistant-stream: active-reader tool arguments (16-char deltas) › 10000 bytes | 2.153ms |  |  | 1.522ms | 2.684ms | 8 |
| tool-args › assistant-stream: active-reader tool arguments (16-char deltas) › 5000 bytes | 1.089ms |  |  | 784.09µs | 1.366ms | 8 |
| tool-args › assistant-stream: complete accumulated arguments (single delta) › 10,000 array elements | 267.99µs |  |  | 245.47µs | 346.51µs | 8 |
| tool-args › assistant-stream: dense accumulated arguments (16-char deltas) › 2,000 array entries | 21.426ms |  |  | 16.472ms | 26.611ms | 8 |
| tool-args › assistant-stream: dense accumulated arguments (16-char deltas) › 2,000 object entries | 480.496ms |  |  | 461.969ms | 850.924ms | 8 |
| tool-args › assistant-stream: execute-only tool arguments (16-char deltas) › 1000 bytes | 189.39µs |  |  | 127.23µs | 237.05µs | 8 |
| tool-args › assistant-stream: execute-only tool arguments (16-char deltas) › 10000 bytes | 1.583ms |  |  | 1.052ms | 1.901ms | 8 |
| tool-args › assistant-stream: execute-only tool arguments (16-char deltas) › 5000 bytes | 803.06µs |  |  | 534.39µs | 976.37µs | 8 |
| tool-args › assistant-stream: long string arguments (4096-char deltas) › accumulator: 10000 bytes | 164.24µs |  |  | 144.39µs | 210.61µs | 8 |
| tool-args › assistant-stream: long string arguments (4096-char deltas) › accumulator: 50000 bytes | 759.64µs |  |  | 686.60µs | 980.26µs | 8 |
| tool-args › assistant-stream: long string arguments (4096-char deltas) › active-reader: 10000 bytes | 180.10µs |  |  | 155.74µs | 231.11µs | 8 |
| tool-args › assistant-stream: long string arguments (4096-char deltas) › active-reader: 50000 bytes | 800.96µs |  |  | 716.23µs | 1.020ms | 8 |
| tree › tree mount+unmount, 500 leaves x 10 hooks › createTapRoot | 2.689ms |  |  | 2.256ms | 3.714ms | 8 |
| tree › tree mount+unmount, 500 leaves x 10 hooks › createTapRootDeps | 2.747ms |  |  | 2.288ms | 3.717ms | 8 |
| tree › tree mount+unmount, 500 leaves x 10 hooks › createTapRootStable | 2.632ms |  |  | 2.221ms | 3.698ms | 8 |
| tree › tree mount+unmount, 500 leaves x 10 hooks › react | 2.652ms |  |  | 2.150ms | 3.726ms | 8 |
| tree › tree mount+unmount, 500 leaves x 10 hooks › tapRoot | 1.704ms |  |  | 1.405ms | 2.350ms | 8 |
| tree › tree update: one leaf dispatch, 500 leaves x 10 hooks › createTapRoot | 2.531ms |  |  | 2.161ms | 3.512ms | 8 |
| tree › tree update: one leaf dispatch, 500 leaves x 10 hooks › createTapRootDeps | 2.528ms |  |  | 2.179ms | 3.507ms | 8 |
| tree › tree update: one leaf dispatch, 500 leaves x 10 hooks › createTapRootStable | 199.38µs |  |  | 166.62µs | 305.20µs | 8 |
| tree › tree update: one leaf dispatch, 500 leaves x 10 hooks › react | 108.60µs |  |  | 94.44µs | 148.10µs | 8 |
| tree › tree update: one leaf dispatch, 500 leaves x 10 hooks › tapRoot | 1.320ms |  |  | 1.108ms | 1.825ms | 8 |
| useResources › useResources mount+unmount, 500 children x 10 hooks › deps | 1.465ms |  |  | 1.185ms | 2.116ms | 8 |
| useResources › useResources mount+unmount, 500 children x 10 hooks › no-deps | 1.533ms |  |  | 1.294ms | 2.162ms | 8 |
| useResources › useResources: one child dispatch, 500 children x 10 hooks › deps | 39.70µs |  |  | 29.71µs | 54.18µs | 8 |
| useResources › useResources: one child dispatch, 500 children x 10 hooks › no-deps | 41.29µs |  |  | 31.55µs | 54.70µs | 8 |
| useResources › useResources: rebuild elements array, 500 children x 10 hooks › deps | 55.66µs |  |  | 45.20µs | 72.42µs | 8 |
| useResources › useResources: rebuild elements array, 500 children x 10 hooks › no-deps | 1.126ms |  |  | 990.30µs | 1.600ms | 8 |

informational; points come from different runners of the same class, so read trends, not single deltas.
