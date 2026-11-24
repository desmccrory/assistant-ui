## aui-perf nightly record

_6 points · 2026-11-19T04:31:14.259Z to 2026-11-24T04:30:35.875Z · latest runner: Intel(R) Xeon(R) 6975P-C · Node v26.13.0_

| bench | latest | Δ7d | Δ30d | min | max | points |
| --- | ---: | ---: | ---: | ---: | ---: | ---: |
| accumulator › assistant-stream: raw controller enqueue overhead › 10,000 chunks from one source stream | 553.61µs |  |  | 553.61µs | 864.27µs | 6 |
| accumulator › assistant-stream: raw controller enqueue overhead › 10,000 controller.enqueue calls | 785.16µs |  |  | 785.16µs | 1.209ms | 6 |
| accumulator › assistant-stream: same 4000-char text, chunk size A/B › 16 deltas × 250 chars | 34.48µs |  |  | 34.48µs | 58.22µs | 6 |
| accumulator › assistant-stream: same 4000-char text, chunk size A/B › 250 deltas × 16 chars | 374.49µs |  |  | 374.49µs | 666.48µs | 6 |
| accumulator › assistant-stream: same 4000-char text, chunk size A/B › 4000 deltas × 1 char (per-token) | 5.844ms |  |  | 5.844ms | 10.380ms | 6 |
| accumulator › assistant-stream: stream + accumulator per-delta cost (16-char deltas) › 100 deltas | 158.84µs |  |  | 158.84µs | 282.75µs | 6 |
| accumulator › assistant-stream: stream + accumulator per-delta cost (16-char deltas) › 1000 deltas | 1.462ms |  |  | 1.462ms | 2.627ms | 6 |
| accumulator › assistant-stream: stream + accumulator per-delta cost (16-char deltas) › 4000 deltas | 5.847ms |  |  | 5.847ms | 10.360ms | 6 |
| accumulator › assistant-stream: stream round trip baseline, no accumulator › 100 deltas | 6.38µs |  |  | 6.33µs | 10.11µs | 6 |
| accumulator › assistant-stream: stream round trip baseline, no accumulator › 1000 deltas | 53.23µs |  |  | 53.23µs | 85.69µs | 6 |
| accumulator › assistant-stream: stream round trip baseline, no accumulator › 4000 deltas | 208.64µs |  |  | 208.64µs | 340.11µs | 6 |
| ai-sdk-system-metadata › ai-sdk: system-message metadata conversion through the runtime › 128 parts, distinct providers (stress) | 54.50µs |  |  | 54.50µs | 137.06µs | 6 |
| ai-sdk-system-metadata › ai-sdk: system-message metadata conversion through the runtime › 16 parts, one repeated provider | 30.09µs |  |  | 30.09µs | 81.72µs | 6 |
| ai-sdk-system-metadata › ai-sdk: system-message metadata conversion through the runtime › 2 parts, one repeated provider | 31.60µs |  |  | 31.57µs | 83.70µs | 6 |
| ai-sdk-system-metadata › ai-sdk: system-message metadata conversion through the runtime › 512 parts, distinct providers (stress) | 198.94µs |  |  | 198.94µs | 318.13µs | 6 |
| ai-sdk-toolkit › ai-sdk: convert fresh AISDKToolkit schemas › 10 static tools | 46.71µs |  |  | 45.77µs | 77.43µs | 6 |
| ai-sdk-toolkit › ai-sdk: convert fresh AISDKToolkit schemas › 100 static tools | 493.35µs |  |  | 479.31µs | 698.64µs | 6 |
| ai-sdk-toolkit › ai-sdk: reuse converted AISDKToolkit schemas › 10 static tools | 6.50µs |  |  | 6.34µs | 10.45µs | 6 |
| ai-sdk-toolkit › ai-sdk: reuse converted AISDKToolkit schemas › 100 static tools | 51.38µs |  |  | 51.38µs | 83.78µs | 6 |
| data-stream › assistant-stream: data stream decode (16-char deltas) › 100 deltas | 442.36µs |  |  | 440.94µs | 760.16µs | 6 |
| data-stream › assistant-stream: data stream decode (16-char deltas) › 1000 deltas | 3.713ms |  |  | 3.713ms | 6.049ms | 6 |
| data-stream › assistant-stream: data stream decode (16-char deltas) › 4000 deltas | 14.430ms |  |  | 14.430ms | 23.946ms | 6 |
| data-stream › assistant-stream: data stream encode (16-char deltas) › 100 deltas | 208.93µs |  |  | 208.30µs | 359.72µs | 6 |
| data-stream › assistant-stream: data stream encode (16-char deltas) › 1000 deltas | 2.039ms |  |  | 2.025ms | 3.455ms | 6 |
| data-stream › assistant-stream: data stream encode (16-char deltas) › 4000 deltas | 8.019ms |  |  | 8.019ms | 13.626ms | 6 |
| external-message-conversion › core: cached external message conversion, one streaming delta › 1000 messages, 6-part replies | 216.47µs |  |  | 204.94µs | 286.73µs | 6 |
| external-message-conversion › core: cached external message conversion, one streaming delta › 5000 messages, 20-part replies | 1.418ms |  |  | 1.388ms | 2.259ms | 6 |
| external-message-conversion › core: external message reasoning continuations › 100 matches | 41.76µs |  |  | 41.76µs | 69.92µs | 6 |
| external-message-conversion › core: external message reasoning continuations › 1000 matches | 421.80µs |  |  | 421.80µs | 710.18µs | 6 |
| external-message-conversion › core: external message reasoning continuations › 5000 matches | 2.271ms |  |  | 2.271ms | 3.843ms | 6 |
| external-message-conversion › core: external message tool results › 100 matches | 53.13µs |  |  | 53.13µs | 79.69µs | 6 |
| external-message-conversion › core: external message tool results › 1000 matches | 529.58µs |  |  | 529.58µs | 794.72µs | 6 |
| external-message-conversion › core: external message tool results › 5000 matches | 2.821ms |  |  | 2.821ms | 4.273ms | 6 |
| external-message-conversion › core: external message unique tool calls › 100 matches | 27.30µs |  |  | 27.30µs | 42.30µs | 6 |
| external-message-conversion › core: external message unique tool calls › 1000 matches | 263.81µs |  |  | 263.81µs | 416.18µs | 6 |
| external-message-conversion › core: external message unique tool calls › 5000 matches | 1.415ms |  |  | 1.415ms | 2.195ms | 6 |
| from-thread-message-like › core: fromThreadMessageLike text parts › 1 text parts | 0.17µs |  |  | 0.17µs | 0.28µs | 6 |
| from-thread-message-like › core: fromThreadMessageLike text parts › 10 text parts | 0.30µs |  |  | 0.30µs | 0.47µs | 6 |
| from-thread-message-like › core: fromThreadMessageLike text parts › 100 text parts | 1.58µs |  |  | 1.58µs | 2.47µs | 6 |
| from-thread-message-like › core: fromThreadMessageLike tool calls › 1 tool calls | 0.39µs |  |  | 0.38µs | 0.68µs | 6 |
| from-thread-message-like › core: fromThreadMessageLike tool calls › 10 tool calls | 2.42µs |  |  | 2.32µs | 3.51µs | 6 |
| from-thread-message-like › core: fromThreadMessageLike tool calls › 100 tool calls | 19.76µs |  |  | 19.76µs | 31.97µs | 6 |
| interactable-array-patches › core: id-keyed interactable array patches › 1000 items and patches | 114.35µs |  |  | 111.19µs | 150.94µs | 6 |
| interactable-array-patches › core: id-keyed interactable array patches › 5000 items and patches | 648.19µs |  |  | 597.75µs | 847.87µs | 6 |
| markdown-preprocess › react-markdown: preprocess › escapeCurrencyDollars, 20,000 tilde runs on one line | 1.983ms |  |  | 1.951ms | 2.807ms | 6 |
| markdown-preprocess › react-markdown: preprocess › escapeCurrencyDollars, 20,000 tildes after prose | 118.95µs |  |  | 118.35µs | 210.03µs | 6 |
| markdown-preprocess › react-markdown: preprocess › escapeCurrencyDollars, 20,000 triple-backtick spans on one line | 2.541ms |  |  | 2.524ms | 3.711ms | 6 |
| markdown-preprocess › react-markdown: preprocess › escapeCurrencyDollars, 5,000 code spans in one paragraph | 345.89µs |  |  | 336.49µs | 513.75µs | 6 |
| markdown-preprocess › react-markdown: preprocess › escapeCurrencyDollars, mixed message, 100 sections | 514.86µs |  |  | 498.64µs | 709.20µs | 6 |
| markdown-preprocess › react-markdown: preprocess › normalizeMathDelimiters, 20,000 tilde runs on one line | 5.795ms |  |  | 5.643ms | 8.157ms | 6 |
| markdown-preprocess › react-markdown: preprocess › normalizeMathDelimiters, 20,000 tildes after prose | 485.57µs |  |  | 483.83µs | 959.53µs | 6 |
| markdown-preprocess › react-markdown: preprocess › normalizeMathDelimiters, 20,000 triple-backtick spans on one line | 14.728ms |  |  | 14.728ms | 23.972ms | 6 |
| markdown-preprocess › react-markdown: preprocess › normalizeMathDelimiters, 5,000 code spans in one paragraph | 2.353ms |  |  | 2.337ms | 3.956ms | 6 |
| markdown-preprocess › react-markdown: preprocess › normalizeMathDelimiters, mixed message, 100 sections | 1.790ms |  |  | 1.766ms | 2.784ms | 6 |
| markdown-streaming › react-markdown: one token after an unchanged fenced code block › 10 KB fenced Markdown | 1.990ms |  |  | 1.986ms | 3.095ms | 6 |
| markdown-streaming › react-markdown: one token after an unchanged fenced code block › 10 KB fenced Markdown deferred | 2.228ms |  |  | 2.194ms | 3.315ms | 6 |
| markdown-streaming › react-markdown: one token after an unchanged fenced code block › 100 KB fenced Markdown | 13.486ms |  |  | 13.415ms | 20.949ms | 6 |
| markdown-streaming › react-markdown: one token after an unchanged fenced code block › 100 KB fenced Markdown deferred | 14.636ms |  |  | 14.636ms | 22.440ms | 6 |
| markdown-streaming › react-markdown: one token changed in the last paragraph, by message length › 1 paragraphs | 1.134ms |  |  | 1.025ms | 1.555ms | 6 |
| markdown-streaming › react-markdown: one token changed in the last paragraph, by message length › 10 paragraphs | 1.943ms |  |  | 1.943ms | 3.130ms | 6 |
| markdown-streaming › react-markdown: one token changed in the last paragraph, by message length › 50 paragraphs | 6.637ms |  |  | 6.479ms | 10.109ms | 6 |
| markdown-streaming › react-markdown: the same token with defer on › 1 paragraphs deferred | 1.254ms |  |  | 1.171ms | 1.468ms | 6 |
| markdown-streaming › react-markdown: the same token with defer on › 10 paragraphs deferred | 1.415ms |  |  | 1.415ms | 1.928ms | 6 |
| markdown-streaming › react-markdown: the same token with defer on › 50 paragraphs deferred | 3.779ms |  |  | 3.698ms | 4.867ms | 6 |
| react-langgraph › react-langgraph: streamed tool argument accumulation › 1000 character argument in 16-character deltas | 200.73µs |  |  | 194.97µs | 345.80µs | 6 |
| react-langgraph › react-langgraph: streamed tool argument accumulation › 10000 character argument in 16-character deltas | 1.625ms |  |  | 1.625ms | 2.851ms | 6 |
| react-langgraph › react-langgraph: streamed tool argument accumulation › 500 short object entries in 16-character deltas | 183.091ms |  |  | 183.091ms | 312.966ms | 6 |
| react-langgraph › react-langgraph: streamed tool argument accumulation › 50000 character argument in 16-character deltas | 8.134ms |  |  | 8.134ms | 13.543ms | 6 |
| react-pi-message-projection › react-pi: streaming tail projection › 10 stable messages | 1.19µs |  |  | 1.19µs | 2.32µs | 6 |
| react-pi-message-projection › react-pi: streaming tail projection › 1000 stable messages | 5.41µs |  |  | 5.40µs | 10.68µs | 6 |
| react-pi-message-projection › react-pi: streaming tail projection › 5000 stable messages | 26.02µs |  |  | 25.73µs | 48.04µs | 6 |
| sse-fragmentation › assistant-stream: fragmented SSE events › 100 KiB, 1 chunks | 4.72µs |  |  | 4.71µs | 7.33µs | 6 |
| sse-fragmentation › assistant-stream: fragmented SSE events › 100 KiB, 101 chunks | 15.54µs |  |  | 15.54µs | 24.21µs | 6 |
| sse-fragmentation › assistant-stream: fragmented SSE events › 1024 KiB, 1 chunks | 45.83µs |  |  | 45.83µs | 64.46µs | 6 |
| sse-fragmentation › assistant-stream: fragmented SSE events › 1024 KiB, 1025 chunks | 192.48µs |  |  | 192.48µs | 344.23µs | 6 |
| thread-scaling › external-store thread: mount+unmount by message count › 10 messages | 4.466ms |  |  | 4.466ms | 6.950ms | 6 |
| thread-scaling › external-store thread: mount+unmount by message count › 100 messages | 26.853ms |  |  | 26.853ms | 45.070ms | 6 |
| thread-scaling › external-store thread: mount+unmount by message count › 1000 messages | 342.834ms |  |  | 320.633ms | 471.630ms | 6 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › 20 message window, 10 messages | 389.24µs |  |  | 389.24µs | 626.18µs | 6 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › 20 message window, 100 messages | 684.54µs |  |  | 642.09µs | 946.59µs | 6 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › 20 message window, 1000 messages | 3.679ms |  |  | 3.138ms | 4.653ms | 6 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › all messages by id, 10 messages | 393.55µs |  |  | 393.55µs | 635.03µs | 6 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › all messages by id, 100 messages | 1.274ms |  |  | 1.079ms | 1.674ms | 6 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › all messages by id, 1000 messages | 8.946ms |  |  | 8.176ms | 15.272ms | 6 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › all messages, 10 messages | 426.72µs |  |  | 345.41µs | 667.45µs | 6 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › all messages, 100 messages | 1.105ms |  |  | 781.80µs | 1.197ms | 6 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › all messages, 1000 messages | 6.034ms |  |  | 5.418ms | 9.906ms | 6 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › provider only, 10 messages | 161.67µs |  |  | 161.45µs | 333.61µs | 6 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › provider only, 100 messages | 401.09µs |  |  | 360.68µs | 544.61µs | 6 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › provider only, 1000 messages | 2.858ms |  |  | 2.329ms | 3.392ms | 6 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › runtime only, 10 messages | 11.18µs |  |  | 11.18µs | 25.72µs | 6 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › runtime only, 100 messages | 22.80µs |  |  | 22.66µs | 40.73µs | 6 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › runtime only, 1000 messages | 195.71µs |  |  | 195.71µs | 306.29µs | 6 |
| thread-scaling › external-store thread: one token changed in the last message, by thread length › 10 messages | 449.34µs |  |  | 392.19µs | 714.62µs | 6 |
| thread-scaling › external-store thread: one token changed in the last message, by thread length › 100 messages | 933.31µs |  |  | 810.46µs | 1.238ms | 6 |
| thread-scaling › external-store thread: one token changed in the last message, by thread length › 1000 messages | 5.845ms |  |  | 5.845ms | 10.929ms | 6 |
| tool-args › assistant-stream: accumulator tool arguments (16-char deltas) › 1000 bytes | 163.10µs |  |  | 162.53µs | 273.57µs | 6 |
| tool-args › assistant-stream: accumulator tool arguments (16-char deltas) › 10000 bytes | 1.479ms |  |  | 1.475ms | 2.358ms | 6 |
| tool-args › assistant-stream: accumulator tool arguments (16-char deltas) › 5000 bytes | 747.95µs |  |  | 747.95µs | 1.191ms | 6 |
| tool-args › assistant-stream: active-reader tool arguments (16-char deltas) › 1000 bytes | 181.16µs |  |  | 181.16µs | 318.76µs | 6 |
| tool-args › assistant-stream: active-reader tool arguments (16-char deltas) › 10000 bytes | 1.579ms |  |  | 1.579ms | 2.684ms | 6 |
| tool-args › assistant-stream: active-reader tool arguments (16-char deltas) › 5000 bytes | 805.97µs |  |  | 800.04µs | 1.366ms | 6 |
| tool-args › assistant-stream: complete accumulated arguments (single delta) › 10,000 array elements | 246.99µs |  |  | 246.99µs | 346.51µs | 6 |
| tool-args › assistant-stream: dense accumulated arguments (16-char deltas) › 2,000 array entries | 16.509ms |  |  | 16.509ms | 26.611ms | 6 |
| tool-args › assistant-stream: dense accumulated arguments (16-char deltas) › 2,000 object entries | 653.406ms |  |  | 461.969ms | 850.924ms | 6 |
| tool-args › assistant-stream: execute-only tool arguments (16-char deltas) › 1000 bytes | 131.58µs |  |  | 130.02µs | 237.05µs | 6 |
| tool-args › assistant-stream: execute-only tool arguments (16-char deltas) › 10000 bytes | 1.078ms |  |  | 1.078ms | 1.901ms | 6 |
| tool-args › assistant-stream: execute-only tool arguments (16-char deltas) › 5000 bytes | 550.61µs |  |  | 542.02µs | 976.37µs | 6 |
| tool-args › assistant-stream: long string arguments (4096-char deltas) › accumulator: 10000 bytes | 148.31µs |  |  | 144.39µs | 210.61µs | 6 |
| tool-args › assistant-stream: long string arguments (4096-char deltas) › accumulator: 50000 bytes | 713.62µs |  |  | 686.60µs | 980.26µs | 6 |
| tool-args › assistant-stream: long string arguments (4096-char deltas) › active-reader: 10000 bytes | 155.83µs |  |  | 155.74µs | 231.11µs | 6 |
| tool-args › assistant-stream: long string arguments (4096-char deltas) › active-reader: 50000 bytes | 737.80µs |  |  | 716.95µs | 1.020ms | 6 |
| tree › tree mount+unmount, 500 leaves x 10 hooks › createTapRoot | 2.276ms |  |  | 2.276ms | 3.714ms | 6 |
| tree › tree mount+unmount, 500 leaves x 10 hooks › createTapRootDeps | 2.329ms |  |  | 2.329ms | 3.717ms | 6 |
| tree › tree mount+unmount, 500 leaves x 10 hooks › createTapRootStable | 2.221ms |  |  | 2.221ms | 3.698ms | 6 |
| tree › tree mount+unmount, 500 leaves x 10 hooks › react | 2.157ms |  |  | 2.157ms | 3.726ms | 6 |
| tree › tree mount+unmount, 500 leaves x 10 hooks › tapRoot | 1.405ms |  |  | 1.405ms | 2.350ms | 6 |
| tree › tree update: one leaf dispatch, 500 leaves x 10 hooks › createTapRoot | 2.210ms |  |  | 2.178ms | 3.512ms | 6 |
| tree › tree update: one leaf dispatch, 500 leaves x 10 hooks › createTapRootDeps | 2.274ms |  |  | 2.213ms | 3.507ms | 6 |
| tree › tree update: one leaf dispatch, 500 leaves x 10 hooks › createTapRootStable | 182.78µs |  |  | 182.78µs | 305.20µs | 6 |
| tree › tree update: one leaf dispatch, 500 leaves x 10 hooks › react | 94.44µs |  |  | 94.44µs | 148.10µs | 6 |
| tree › tree update: one leaf dispatch, 500 leaves x 10 hooks › tapRoot | 1.154ms |  |  | 1.132ms | 1.825ms | 6 |
| useResources › useResources mount+unmount, 500 children x 10 hooks › deps | 1.212ms |  |  | 1.212ms | 2.116ms | 6 |
| useResources › useResources mount+unmount, 500 children x 10 hooks › no-deps | 1.308ms |  |  | 1.308ms | 2.162ms | 6 |
| useResources › useResources: one child dispatch, 500 children x 10 hooks › deps | 30.01µs |  |  | 29.89µs | 54.18µs | 6 |
| useResources › useResources: one child dispatch, 500 children x 10 hooks › no-deps | 32.54µs |  |  | 32.50µs | 54.70µs | 6 |
| useResources › useResources: rebuild elements array, 500 children x 10 hooks › deps | 47.02µs |  |  | 46.72µs | 72.42µs | 6 |
| useResources › useResources: rebuild elements array, 500 children x 10 hooks › no-deps | 1.025ms |  |  | 1.025ms | 1.600ms | 6 |

informational; points come from different runners of the same class, so read trends, not single deltas.
