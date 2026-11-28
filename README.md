## aui-perf nightly record

_10 points · 2026-11-19T04:31:14.259Z to 2026-11-28T04:29:42.280Z · latest runner: AMD EPYC 9V74 80-Core Processor · Node v26.13.0_

| bench | latest | Δ7d | Δ30d | min | max | points |
| --- | ---: | ---: | ---: | ---: | ---: | ---: |
| accumulator › assistant-stream: raw controller enqueue overhead › 10,000 chunks from one source stream | 694.34µs | +3.3% |  | 541.80µs | 864.27µs | 10 |
| accumulator › assistant-stream: raw controller enqueue overhead › 10,000 controller.enqueue calls | 1.008ms | +3.2% |  | 767.53µs | 1.209ms | 10 |
| accumulator › assistant-stream: same 4000-char text, chunk size A/B › 16 deltas × 250 chars | 44.28µs | +0.3% |  | 34.48µs | 58.22µs | 10 |
| accumulator › assistant-stream: same 4000-char text, chunk size A/B › 250 deltas × 16 chars | 521.87µs | +1.9% |  | 372.90µs | 666.48µs | 10 |
| accumulator › assistant-stream: same 4000-char text, chunk size A/B › 4000 deltas × 1 char (per-token) | 8.089ms | +1.7% |  | 5.831ms | 10.380ms | 10 |
| accumulator › assistant-stream: stream + accumulator per-delta cost (16-char deltas) › 100 deltas | 218.23µs | +1.7% |  | 155.31µs | 282.75µs | 10 |
| accumulator › assistant-stream: stream + accumulator per-delta cost (16-char deltas) › 1000 deltas | 2.012ms | -0.1% |  | 1.427ms | 2.627ms | 10 |
| accumulator › assistant-stream: stream + accumulator per-delta cost (16-char deltas) › 4000 deltas | 8.093ms | +3.1% |  | 5.729ms | 10.360ms | 10 |
| accumulator › assistant-stream: stream round trip baseline, no accumulator › 100 deltas | 8.20µs | +2.3% |  | 6.19µs | 10.11µs | 10 |
| accumulator › assistant-stream: stream round trip baseline, no accumulator › 1000 deltas | 68.73µs | +3.0% |  | 52.27µs | 85.69µs | 10 |
| accumulator › assistant-stream: stream round trip baseline, no accumulator › 4000 deltas | 270.22µs | +3.5% |  | 208.27µs | 340.11µs | 10 |
| ai-sdk-system-metadata › ai-sdk: system-message metadata conversion through the runtime › 128 parts, distinct providers (stress) | 79.96µs | -0.3% |  | 54.50µs | 137.06µs | 10 |
| ai-sdk-system-metadata › ai-sdk: system-message metadata conversion through the runtime › 16 parts, one repeated provider | 42.87µs | +1.9% |  | 29.89µs | 81.72µs | 10 |
| ai-sdk-system-metadata › ai-sdk: system-message metadata conversion through the runtime › 2 parts, one repeated provider | 41.33µs | -0.8% |  | 31.36µs | 83.70µs | 10 |
| ai-sdk-system-metadata › ai-sdk: system-message metadata conversion through the runtime › 512 parts, distinct providers (stress) | 249.68µs | +2.6% |  | 198.94µs | 318.13µs | 10 |
| ai-sdk-toolkit › ai-sdk: convert fresh AISDKToolkit schemas › 10 static tools | 52.70µs | +0.2% |  | 44.45µs | 77.43µs | 10 |
| ai-sdk-toolkit › ai-sdk: convert fresh AISDKToolkit schemas › 100 static tools | 511.56µs | -2.4% |  | 479.31µs | 698.64µs | 10 |
| ai-sdk-toolkit › ai-sdk: reuse converted AISDKToolkit schemas › 10 static tools | 7.54µs | +1.3% |  | 6.09µs | 10.45µs | 10 |
| ai-sdk-toolkit › ai-sdk: reuse converted AISDKToolkit schemas › 100 static tools | 60.81µs | +0.3% |  | 51.38µs | 83.78µs | 10 |
| data-stream › assistant-stream: data stream decode (16-char deltas) › 100 deltas | 589.44µs | +0.9% |  | 430.55µs | 760.16µs | 10 |
| data-stream › assistant-stream: data stream decode (16-char deltas) › 1000 deltas | 4.974ms | -0.1% |  | 3.635ms | 6.049ms | 10 |
| data-stream › assistant-stream: data stream decode (16-char deltas) › 4000 deltas | 19.497ms | -0.7% |  | 14.176ms | 23.946ms | 10 |
| data-stream › assistant-stream: data stream encode (16-char deltas) › 100 deltas | 284.45µs | -0.3% |  | 203.67µs | 359.72µs | 10 |
| data-stream › assistant-stream: data stream encode (16-char deltas) › 1000 deltas | 2.773ms | +0.7% |  | 1.965ms | 3.455ms | 10 |
| data-stream › assistant-stream: data stream encode (16-char deltas) › 4000 deltas | 11.051ms | +1.7% |  | 8.019ms | 13.626ms | 10 |
| external-message-conversion › core: cached external message conversion, one streaming delta › 1000 messages, 6-part replies | 214.15µs | -1.2% |  | 204.94µs | 286.73µs | 10 |
| external-message-conversion › core: cached external message conversion, one streaming delta › 5000 messages, 20-part replies | 1.746ms | +25.8% |  | 1.276ms | 2.259ms | 10 |
| external-message-conversion › core: external message reasoning continuations › 100 matches | 50.36µs | +0.5% |  | 41.62µs | 69.92µs | 10 |
| external-message-conversion › core: external message reasoning continuations › 1000 matches | 507.75µs | +0.4% |  | 415.52µs | 710.18µs | 10 |
| external-message-conversion › core: external message reasoning continuations › 5000 matches | 2.688ms | -0.0% |  | 2.235ms | 3.843ms | 10 |
| external-message-conversion › core: external message tool results › 100 matches | 59.55µs | -0.3% |  | 52.57µs | 79.69µs | 10 |
| external-message-conversion › core: external message tool results › 1000 matches | 603.62µs | +0.4% |  | 526.93µs | 794.72µs | 10 |
| external-message-conversion › core: external message tool results › 5000 matches | 3.154ms | +0.2% |  | 2.771ms | 4.273ms | 10 |
| external-message-conversion › core: external message unique tool calls › 100 matches | 31.76µs | +1.9% |  | 27.14µs | 42.30µs | 10 |
| external-message-conversion › core: external message unique tool calls › 1000 matches | 306.39µs | +3.4% |  | 253.31µs | 416.18µs | 10 |
| external-message-conversion › core: external message unique tool calls › 5000 matches | 1.635ms | +0.8% |  | 1.368ms | 2.195ms | 10 |
| from-thread-message-like › core: fromThreadMessageLike text parts › 1 text parts | 0.21µs | -0.5% |  | 0.17µs | 0.28µs | 10 |
| from-thread-message-like › core: fromThreadMessageLike text parts › 10 text parts | 0.38µs | +1.8% |  | 0.30µs | 0.47µs | 10 |
| from-thread-message-like › core: fromThreadMessageLike text parts › 100 text parts | 2.11µs | +0.3% |  | 1.58µs | 2.47µs | 10 |
| from-thread-message-like › core: fromThreadMessageLike tool calls › 1 tool calls | 0.49µs | +2.0% |  | 0.38µs | 0.68µs | 10 |
| from-thread-message-like › core: fromThreadMessageLike tool calls › 10 tool calls | 2.53µs | +3.7% |  | 2.23µs | 3.51µs | 10 |
| from-thread-message-like › core: fromThreadMessageLike tool calls › 100 tool calls | 23.42µs | +4.2% |  | 19.76µs | 31.97µs | 10 |
| interactable-array-patches › core: id-keyed interactable array patches › 1000 items and patches | 114.48µs | +3.0% |  | 111.19µs | 150.94µs | 10 |
| interactable-array-patches › core: id-keyed interactable array patches › 5000 items and patches | 593.83µs | -0.7% |  | 593.83µs | 847.87µs | 10 |
| markdown-preprocess › react-markdown: preprocess › escapeCurrencyDollars, 20,000 tilde runs on one line | 2.118ms | +0.1% |  | 1.951ms | 2.807ms | 10 |
| markdown-preprocess › react-markdown: preprocess › escapeCurrencyDollars, 20,000 tildes after prose | 160.71µs | -0.1% |  | 118.35µs | 210.03µs | 10 |
| markdown-preprocess › react-markdown: preprocess › escapeCurrencyDollars, 20,000 triple-backtick spans on one line | 2.746ms | -0.1% |  | 2.524ms | 3.711ms | 10 |
| markdown-preprocess › react-markdown: preprocess › escapeCurrencyDollars, 5,000 code spans in one paragraph | 389.86µs | +9.5% |  | 336.49µs | 513.75µs | 10 |
| markdown-preprocess › react-markdown: preprocess › escapeCurrencyDollars, mixed message, 100 sections | 505.86µs | +1.4% |  | 498.64µs | 709.20µs | 10 |
| markdown-preprocess › react-markdown: preprocess › normalizeMathDelimiters, 20,000 tilde runs on one line | 6.105ms | +8.2% |  | 5.643ms | 8.157ms | 10 |
| markdown-preprocess › react-markdown: preprocess › normalizeMathDelimiters, 20,000 tildes after prose | 739.36µs | -2.8% |  | 482.66µs | 959.53µs | 10 |
| markdown-preprocess › react-markdown: preprocess › normalizeMathDelimiters, 20,000 triple-backtick spans on one line | 16.312ms | +0.4% |  | 14.666ms | 23.972ms | 10 |
| markdown-preprocess › react-markdown: preprocess › normalizeMathDelimiters, 5,000 code spans in one paragraph | 2.741ms | +0.6% |  | 2.308ms | 3.956ms | 10 |
| markdown-preprocess › react-markdown: preprocess › normalizeMathDelimiters, mixed message, 100 sections | 1.952ms | +1.1% |  | 1.766ms | 2.784ms | 10 |
| markdown-streaming › react-markdown: one token after an unchanged fenced code block › 10 KB fenced Markdown | 2.320ms | +0.7% |  | 1.972ms | 3.095ms | 10 |
| markdown-streaming › react-markdown: one token after an unchanged fenced code block › 10 KB fenced Markdown deferred | 2.459ms | -1.2% |  | 2.186ms | 3.315ms | 10 |
| markdown-streaming › react-markdown: one token after an unchanged fenced code block › 100 KB fenced Markdown | 16.680ms | -1.5% |  | 13.415ms | 20.949ms | 10 |
| markdown-streaming › react-markdown: one token after an unchanged fenced code block › 100 KB fenced Markdown deferred | 18.094ms | +0.6% |  | 14.636ms | 22.440ms | 10 |
| markdown-streaming › react-markdown: one token changed in the last paragraph, by message length › 1 paragraphs | 1.035ms | +0.9% |  | 1.025ms | 1.555ms | 10 |
| markdown-streaming › react-markdown: one token changed in the last paragraph, by message length › 10 paragraphs | 2.147ms | +1.3% |  | 1.848ms | 3.130ms | 10 |
| markdown-streaming › react-markdown: one token changed in the last paragraph, by message length › 50 paragraphs | 7.444ms | -0.0% |  | 6.313ms | 10.109ms | 10 |
| markdown-streaming › react-markdown: the same token with defer on › 1 paragraphs deferred | 1.422ms | -3.1% |  | 1.171ms | 1.524ms | 10 |
| markdown-streaming › react-markdown: the same token with defer on › 10 paragraphs deferred | 1.502ms | +5.7% |  | 1.395ms | 1.928ms | 10 |
| markdown-streaming › react-markdown: the same token with defer on › 50 paragraphs deferred | 4.312ms | +3.4% |  | 3.206ms | 4.867ms | 10 |
| react-langgraph › react-langgraph: streamed tool argument accumulation › 1000 character argument in 16-character deltas | 253.85µs | +0.3% |  | 194.97µs | 345.80µs | 10 |
| react-langgraph › react-langgraph: streamed tool argument accumulation › 10000 character argument in 16-character deltas | 2.089ms | -0.0% |  | 1.616ms | 2.851ms | 10 |
| react-langgraph › react-langgraph: streamed tool argument accumulation › 500 short object entries in 16-character deltas | 214.410ms | +1.3% |  | 181.912ms | 312.966ms | 10 |
| react-langgraph › react-langgraph: streamed tool argument accumulation › 50000 character argument in 16-character deltas | 10.100ms | -2.5% |  | 7.867ms | 13.543ms | 10 |
| react-pi-message-projection › react-pi: streaming tail projection › 10 stable messages | 1.84µs | +3.2% |  | 1.18µs | 2.32µs | 10 |
| react-pi-message-projection › react-pi: streaming tail projection › 1000 stable messages | 9.31µs | +4.6% |  | 5.40µs | 10.68µs | 10 |
| react-pi-message-projection › react-pi: streaming tail projection › 5000 stable messages | 36.08µs | +3.3% |  | 25.29µs | 48.04µs | 10 |
| sse-fragmentation › assistant-stream: fragmented SSE events › 100 KiB, 1 chunks | 7.33µs | +0.1% |  | 4.70µs | 7.35µs | 10 |
| sse-fragmentation › assistant-stream: fragmented SSE events › 100 KiB, 101 chunks | 19.06µs | -1.9% |  | 15.35µs | 24.21µs | 10 |
| sse-fragmentation › assistant-stream: fragmented SSE events › 1024 KiB, 1 chunks | 72.50µs | +14.1% |  | 45.83µs | 72.66µs | 10 |
| sse-fragmentation › assistant-stream: fragmented SSE events › 1024 KiB, 1025 chunks | 246.15µs | +4.9% |  | 183.03µs | 344.23µs | 10 |
| thread-scaling › external-store thread: mount+unmount by message count › 10 messages | 4.612ms | +2.0% |  | 3.941ms | 6.950ms | 10 |
| thread-scaling › external-store thread: mount+unmount by message count › 100 messages | 29.973ms | +0.7% |  | 22.883ms | 45.070ms | 10 |
| thread-scaling › external-store thread: mount+unmount by message count › 1000 messages | 383.839ms | +1.9% |  | 303.432ms | 471.630ms | 10 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › 20 message window, 10 messages | 488.56µs | +12.8% |  | 329.18µs | 626.18µs | 10 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › 20 message window, 100 messages | 741.59µs | +7.6% |  | 635.87µs | 946.59µs | 10 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › 20 message window, 1000 messages | 3.234ms | -3.2% |  | 2.761ms | 4.653ms | 10 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › all messages by id, 10 messages | 484.24µs | +3.4% |  | 336.50µs | 635.03µs | 10 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › all messages by id, 100 messages | 1.129ms | +4.6% |  | 1.079ms | 1.674ms | 10 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › all messages by id, 1000 messages | 10.538ms | +0.8% |  | 8.034ms | 15.272ms | 10 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › all messages, 10 messages | 468.68µs | +15.0% |  | 311.25µs | 667.45µs | 10 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › all messages, 100 messages | 893.87µs | +14.3% |  | 781.80µs | 1.197ms | 10 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › all messages, 1000 messages | 5.960ms | -4.5% |  | 5.241ms | 9.906ms | 10 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › provider only, 10 messages | 250.22µs | -0.5% |  | 145.04µs | 333.61µs | 10 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › provider only, 100 messages | 429.35µs | +7.1% |  | 359.63µs | 544.61µs | 10 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › provider only, 1000 messages | 2.695ms | +15.7% |  | 2.329ms | 3.392ms | 10 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › runtime only, 10 messages | 12.86µs | +2.0% |  | 10.93µs | 25.72µs | 10 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › runtime only, 100 messages | 26.69µs | +1.5% |  | 22.08µs | 40.73µs | 10 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › runtime only, 1000 messages | 199.92µs | +2.1% |  | 183.75µs | 306.29µs | 10 |
| thread-scaling › external-store thread: one token changed in the last message, by thread length › 10 messages | 445.13µs | +1.4% |  | 392.19µs | 714.62µs | 10 |
| thread-scaling › external-store thread: one token changed in the last message, by thread length › 100 messages | 820.33µs | +1.2% |  | 810.46µs | 1.238ms | 10 |
| thread-scaling › external-store thread: one token changed in the last message, by thread length › 1000 messages | 6.333ms | +7.6% |  | 5.162ms | 10.929ms | 10 |
| tool-args › assistant-stream: accumulator tool arguments (16-char deltas) › 1000 bytes | 200.20µs | +1.7% |  | 156.10µs | 273.57µs | 10 |
| tool-args › assistant-stream: accumulator tool arguments (16-char deltas) › 10000 bytes | 1.794ms | +0.8% |  | 1.447ms | 2.358ms | 10 |
| tool-args › assistant-stream: accumulator tool arguments (16-char deltas) › 5000 bytes | 899.66µs | +0.3% |  | 724.66µs | 1.191ms | 10 |
| tool-args › assistant-stream: active-reader tool arguments (16-char deltas) › 1000 bytes | 240.72µs | +1.1% |  | 175.27µs | 318.76µs | 10 |
| tool-args › assistant-stream: active-reader tool arguments (16-char deltas) › 10000 bytes | 2.126ms | +1.3% |  | 1.522ms | 2.684ms | 10 |
| tool-args › assistant-stream: active-reader tool arguments (16-char deltas) › 5000 bytes | 1.075ms | +1.6% |  | 784.09µs | 1.366ms | 10 |
| tool-args › assistant-stream: complete accumulated arguments (single delta) › 10,000 array elements | 265.41µs | -0.1% |  | 245.47µs | 346.51µs | 10 |
| tool-args › assistant-stream: dense accumulated arguments (16-char deltas) › 2,000 array entries | 20.671ms | +1.0% |  | 16.472ms | 26.611ms | 10 |
| tool-args › assistant-stream: dense accumulated arguments (16-char deltas) › 2,000 object entries | 469.585ms | +1.6% |  | 461.969ms | 850.924ms | 10 |
| tool-args › assistant-stream: execute-only tool arguments (16-char deltas) › 1000 bytes | 187.82µs | +1.8% |  | 127.23µs | 237.05µs | 10 |
| tool-args › assistant-stream: execute-only tool arguments (16-char deltas) › 10000 bytes | 1.557ms | +0.9% |  | 1.052ms | 1.901ms | 10 |
| tool-args › assistant-stream: execute-only tool arguments (16-char deltas) › 5000 bytes | 796.03µs | +1.3% |  | 534.39µs | 976.37µs | 10 |
| tool-args › assistant-stream: long string arguments (4096-char deltas) › accumulator: 10000 bytes | 162.66µs | +0.1% |  | 144.39µs | 210.61µs | 10 |
| tool-args › assistant-stream: long string arguments (4096-char deltas) › accumulator: 50000 bytes | 766.10µs | +0.5% |  | 686.60µs | 980.26µs | 10 |
| tool-args › assistant-stream: long string arguments (4096-char deltas) › active-reader: 10000 bytes | 178.76µs | +0.6% |  | 155.74µs | 231.11µs | 10 |
| tool-args › assistant-stream: long string arguments (4096-char deltas) › active-reader: 50000 bytes | 792.11µs | -0.1% |  | 716.23µs | 1.020ms | 10 |
| tree › tree mount+unmount, 500 leaves x 10 hooks › createTapRoot | 2.625ms | +0.1% |  | 2.256ms | 3.714ms | 10 |
| tree › tree mount+unmount, 500 leaves x 10 hooks › createTapRootDeps | 2.673ms | +0.1% |  | 2.288ms | 3.717ms | 10 |
| tree › tree mount+unmount, 500 leaves x 10 hooks › createTapRootStable | 2.581ms | -0.9% |  | 2.221ms | 3.698ms | 10 |
| tree › tree mount+unmount, 500 leaves x 10 hooks › react | 2.685ms | +1.2% |  | 2.150ms | 3.726ms | 10 |
| tree › tree mount+unmount, 500 leaves x 10 hooks › tapRoot | 1.671ms | -0.3% |  | 1.405ms | 2.350ms | 10 |
| tree › tree update: one leaf dispatch, 500 leaves x 10 hooks › createTapRoot | 2.509ms | +0.7% |  | 2.161ms | 3.512ms | 10 |
| tree › tree update: one leaf dispatch, 500 leaves x 10 hooks › createTapRootDeps | 2.506ms | +0.9% |  | 2.179ms | 3.507ms | 10 |
| tree › tree update: one leaf dispatch, 500 leaves x 10 hooks › createTapRootStable | 235.67µs | +21.0% |  | 166.62µs | 305.20µs | 10 |
| tree › tree update: one leaf dispatch, 500 leaves x 10 hooks › react | 106.88µs | -1.3% |  | 94.44µs | 148.10µs | 10 |
| tree › tree update: one leaf dispatch, 500 leaves x 10 hooks › tapRoot | 1.306ms | -1.6% |  | 1.108ms | 1.825ms | 10 |
| useResources › useResources mount+unmount, 500 children x 10 hooks › deps | 1.416ms | -2.2% |  | 1.185ms | 2.116ms | 10 |
| useResources › useResources mount+unmount, 500 children x 10 hooks › no-deps | 1.459ms | -4.4% |  | 1.294ms | 2.162ms | 10 |
| useResources › useResources: one child dispatch, 500 children x 10 hooks › deps | 38.50µs | +2.7% |  | 29.71µs | 54.18µs | 10 |
| useResources › useResources: one child dispatch, 500 children x 10 hooks › no-deps | 40.15µs | +0.4% |  | 31.55µs | 54.70µs | 10 |
| useResources › useResources: rebuild elements array, 500 children x 10 hooks › deps | 54.81µs | +2.9% |  | 45.20µs | 72.42µs | 10 |
| useResources › useResources: rebuild elements array, 500 children x 10 hooks › no-deps | 1.098ms | -4.3% |  | 990.30µs | 1.600ms | 10 |

informational; points come from different runners of the same class, so read trends, not single deltas.
