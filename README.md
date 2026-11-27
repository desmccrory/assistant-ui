## aui-perf nightly record

_9 points · 2026-11-19T04:31:14.259Z to 2026-11-27T04:30:54.708Z · latest runner: INTEL(R) XEON(R) PLATINUM 8573C · Node v26.13.0_

| bench | latest | Δ7d | Δ30d | min | max | points |
| --- | ---: | ---: | ---: | ---: | ---: | ---: |
| accumulator › assistant-stream: raw controller enqueue overhead › 10,000 chunks from one source stream | 634.84µs | +14.1% |  | 541.80µs | 864.27µs | 9 |
| accumulator › assistant-stream: raw controller enqueue overhead › 10,000 controller.enqueue calls | 944.18µs | +19.1% |  | 767.53µs | 1.209ms | 9 |
| accumulator › assistant-stream: same 4000-char text, chunk size A/B › 16 deltas × 250 chars | 45.41µs | +27.5% |  | 34.48µs | 58.22µs | 9 |
| accumulator › assistant-stream: same 4000-char text, chunk size A/B › 250 deltas × 16 chars | 522.47µs | +34.0% |  | 372.90µs | 666.48µs | 9 |
| accumulator › assistant-stream: same 4000-char text, chunk size A/B › 4000 deltas × 1 char (per-token) | 8.237ms | +36.8% |  | 5.831ms | 10.380ms | 9 |
| accumulator › assistant-stream: stream + accumulator per-delta cost (16-char deltas) › 100 deltas | 221.99µs | +35.6% |  | 155.31µs | 282.75µs | 9 |
| accumulator › assistant-stream: stream + accumulator per-delta cost (16-char deltas) › 1000 deltas | 1.967ms | +33.4% |  | 1.427ms | 2.627ms | 9 |
| accumulator › assistant-stream: stream + accumulator per-delta cost (16-char deltas) › 4000 deltas | 7.969ms | +34.1% |  | 5.729ms | 10.360ms | 9 |
| accumulator › assistant-stream: stream round trip baseline, no accumulator › 100 deltas | 7.57µs | +19.5% |  | 6.19µs | 10.11µs | 9 |
| accumulator › assistant-stream: stream round trip baseline, no accumulator › 1000 deltas | 62.30µs | +16.6% |  | 52.27µs | 85.69µs | 9 |
| accumulator › assistant-stream: stream round trip baseline, no accumulator › 4000 deltas | 243.67µs | +15.7% |  | 208.27µs | 340.11µs | 9 |
| ai-sdk-system-metadata › ai-sdk: system-message metadata conversion through the runtime › 128 parts, distinct providers (stress) | 69.62µs | +27.5% |  | 54.50µs | 137.06µs | 9 |
| ai-sdk-system-metadata › ai-sdk: system-message metadata conversion through the runtime › 16 parts, one repeated provider | 36.73µs | +20.4% |  | 29.89µs | 81.72µs | 9 |
| ai-sdk-system-metadata › ai-sdk: system-message metadata conversion through the runtime › 2 parts, one repeated provider | 38.43µs | +21.7% |  | 31.36µs | 83.70µs | 9 |
| ai-sdk-system-metadata › ai-sdk: system-message metadata conversion through the runtime › 512 parts, distinct providers (stress) | 227.43µs | +13.3% |  | 198.94µs | 318.13µs | 9 |
| ai-sdk-toolkit › ai-sdk: convert fresh AISDKToolkit schemas › 10 static tools | 57.52µs | +25.7% |  | 44.45µs | 77.43µs | 9 |
| ai-sdk-toolkit › ai-sdk: convert fresh AISDKToolkit schemas › 100 static tools | 552.23µs | +15.2% |  | 479.31µs | 698.64µs | 9 |
| ai-sdk-toolkit › ai-sdk: reuse converted AISDKToolkit schemas › 10 static tools | 7.76µs | +22.4% |  | 6.09µs | 10.45µs | 9 |
| ai-sdk-toolkit › ai-sdk: reuse converted AISDKToolkit schemas › 100 static tools | 62.25µs | +15.8% |  | 51.38µs | 83.78µs | 9 |
| data-stream › assistant-stream: data stream decode (16-char deltas) › 100 deltas | 541.86µs | +22.9% |  | 430.55µs | 760.16µs | 9 |
| data-stream › assistant-stream: data stream decode (16-char deltas) › 1000 deltas | 4.474ms | +19.6% |  | 3.635ms | 6.049ms | 9 |
| data-stream › assistant-stream: data stream decode (16-char deltas) › 4000 deltas | 17.333ms | +18.8% |  | 14.176ms | 23.946ms | 9 |
| data-stream › assistant-stream: data stream encode (16-char deltas) › 100 deltas | 254.13µs | +22.0% |  | 203.67µs | 359.72µs | 9 |
| data-stream › assistant-stream: data stream encode (16-char deltas) › 1000 deltas | 2.535ms | +25.2% |  | 1.965ms | 3.455ms | 9 |
| data-stream › assistant-stream: data stream encode (16-char deltas) › 4000 deltas | 9.801ms | +20.0% |  | 8.019ms | 13.626ms | 9 |
| external-message-conversion › core: cached external message conversion, one streaming delta › 1000 messages, 6-part replies | 223.53µs | +9.1% |  | 204.94µs | 286.73µs | 9 |
| external-message-conversion › core: cached external message conversion, one streaming delta › 5000 messages, 20-part replies | 1.947ms | +3.7% |  | 1.276ms | 2.259ms | 9 |
| external-message-conversion › core: external message reasoning continuations › 100 matches | 53.42µs | +25.5% |  | 41.62µs | 69.92µs | 9 |
| external-message-conversion › core: external message reasoning continuations › 1000 matches | 524.32µs | +21.6% |  | 415.52µs | 710.18µs | 9 |
| external-message-conversion › core: external message reasoning continuations › 5000 matches | 2.748ms | +18.1% |  | 2.235ms | 3.843ms | 9 |
| external-message-conversion › core: external message tool results › 100 matches | 62.62µs | +16.0% |  | 52.57µs | 79.69µs | 9 |
| external-message-conversion › core: external message tool results › 1000 matches | 618.23µs | +13.2% |  | 526.93µs | 794.72µs | 9 |
| external-message-conversion › core: external message tool results › 5000 matches | 3.308ms | +16.9% |  | 2.771ms | 4.273ms | 9 |
| external-message-conversion › core: external message unique tool calls › 100 matches | 32.34µs | +15.1% |  | 27.14µs | 42.30µs | 9 |
| external-message-conversion › core: external message unique tool calls › 1000 matches | 308.28µs | +15.0% |  | 253.31µs | 416.18µs | 9 |
| external-message-conversion › core: external message unique tool calls › 5000 matches | 1.606ms | +12.9% |  | 1.368ms | 2.195ms | 9 |
| from-thread-message-like › core: fromThreadMessageLike text parts › 1 text parts | 0.20µs | +14.7% |  | 0.17µs | 0.28µs | 9 |
| from-thread-message-like › core: fromThreadMessageLike text parts › 10 text parts | 0.36µs | +19.8% |  | 0.30µs | 0.47µs | 9 |
| from-thread-message-like › core: fromThreadMessageLike text parts › 100 text parts | 1.83µs | +15.3% |  | 1.58µs | 2.47µs | 9 |
| from-thread-message-like › core: fromThreadMessageLike tool calls › 1 tool calls | 0.47µs | +21.8% |  | 0.38µs | 0.68µs | 9 |
| from-thread-message-like › core: fromThreadMessageLike tool calls › 10 tool calls | 2.65µs | +14.3% |  | 2.23µs | 3.51µs | 9 |
| from-thread-message-like › core: fromThreadMessageLike tool calls › 100 tool calls | 24.11µs | +20.0% |  | 19.76µs | 31.97µs | 9 |
| interactable-array-patches › core: id-keyed interactable array patches › 1000 items and patches | 135.69µs | +18.9% |  | 111.19µs | 150.94µs | 9 |
| interactable-array-patches › core: id-keyed interactable array patches › 5000 items and patches | 749.00µs | +18.5% |  | 597.75µs | 847.87µs | 9 |
| markdown-preprocess › react-markdown: preprocess › escapeCurrencyDollars, 20,000 tilde runs on one line | 2.614ms | +34.0% |  | 1.951ms | 2.807ms | 9 |
| markdown-preprocess › react-markdown: preprocess › escapeCurrencyDollars, 20,000 tildes after prose | 196.86µs | +66.3% |  | 118.35µs | 210.03µs | 9 |
| markdown-preprocess › react-markdown: preprocess › escapeCurrencyDollars, 20,000 triple-backtick spans on one line | 3.367ms | +33.4% |  | 2.524ms | 3.711ms | 9 |
| markdown-preprocess › react-markdown: preprocess › escapeCurrencyDollars, 5,000 code spans in one paragraph | 416.69µs | +23.8% |  | 336.49µs | 513.75µs | 9 |
| markdown-preprocess › react-markdown: preprocess › escapeCurrencyDollars, mixed message, 100 sections | 590.58µs | +18.4% |  | 498.64µs | 709.20µs | 9 |
| markdown-preprocess › react-markdown: preprocess › normalizeMathDelimiters, 20,000 tilde runs on one line | 7.508ms | +30.2% |  | 5.643ms | 8.157ms | 9 |
| markdown-preprocess › react-markdown: preprocess › normalizeMathDelimiters, 20,000 tildes after prose | 885.69µs | +83.1% |  | 482.66µs | 959.53µs | 9 |
| markdown-preprocess › react-markdown: preprocess › normalizeMathDelimiters, 20,000 triple-backtick spans on one line | 18.026ms | +21.5% |  | 14.666ms | 23.972ms | 9 |
| markdown-preprocess › react-markdown: preprocess › normalizeMathDelimiters, 5,000 code spans in one paragraph | 2.881ms | +23.3% |  | 2.308ms | 3.956ms | 9 |
| markdown-preprocess › react-markdown: preprocess › normalizeMathDelimiters, mixed message, 100 sections | 2.215ms | +25.4% |  | 1.766ms | 2.784ms | 9 |
| markdown-streaming › react-markdown: one token after an unchanged fenced code block › 10 KB fenced Markdown | 2.623ms | +32.1% |  | 1.972ms | 3.095ms | 9 |
| markdown-streaming › react-markdown: one token after an unchanged fenced code block › 10 KB fenced Markdown deferred | 2.760ms | +25.8% |  | 2.186ms | 3.315ms | 9 |
| markdown-streaming › react-markdown: one token after an unchanged fenced code block › 100 KB fenced Markdown | 17.546ms | +30.8% |  | 13.415ms | 20.949ms | 9 |
| markdown-streaming › react-markdown: one token after an unchanged fenced code block › 100 KB fenced Markdown deferred | 18.990ms | +29.5% |  | 14.636ms | 22.440ms | 9 |
| markdown-streaming › react-markdown: one token changed in the last paragraph, by message length › 1 paragraphs | 1.433ms | +25.9% |  | 1.025ms | 1.555ms | 9 |
| markdown-streaming › react-markdown: one token changed in the last paragraph, by message length › 10 paragraphs | 2.652ms | +36.3% |  | 1.848ms | 3.130ms | 9 |
| markdown-streaming › react-markdown: one token changed in the last paragraph, by message length › 50 paragraphs | 7.938ms | +22.5% |  | 6.313ms | 10.109ms | 9 |
| markdown-streaming › react-markdown: the same token with defer on › 1 paragraphs deferred | 1.284ms | -11.3% |  | 1.171ms | 1.524ms | 9 |
| markdown-streaming › react-markdown: the same token with defer on › 10 paragraphs deferred | 1.591ms | +8.9% |  | 1.395ms | 1.928ms | 9 |
| markdown-streaming › react-markdown: the same token with defer on › 50 paragraphs deferred | 4.765ms | +28.9% |  | 3.206ms | 4.867ms | 9 |
| react-langgraph › react-langgraph: streamed tool argument accumulation › 1000 character argument in 16-character deltas | 254.22µs | +30.4% |  | 194.97µs | 345.80µs | 9 |
| react-langgraph › react-langgraph: streamed tool argument accumulation › 10000 character argument in 16-character deltas | 2.048ms | +22.6% |  | 1.616ms | 2.851ms | 9 |
| react-langgraph › react-langgraph: streamed tool argument accumulation › 500 short object entries in 16-character deltas | 222.279ms | +20.3% |  | 181.912ms | 312.966ms | 9 |
| react-langgraph › react-langgraph: streamed tool argument accumulation › 50000 character argument in 16-character deltas | 9.629ms | +15.5% |  | 7.867ms | 13.543ms | 9 |
| react-pi-message-projection › react-pi: streaming tail projection › 10 stable messages | 1.75µs | +44.0% |  | 1.18µs | 2.32µs | 9 |
| react-pi-message-projection › react-pi: streaming tail projection › 1000 stable messages | 6.19µs | +14.7% |  | 5.40µs | 10.68µs | 9 |
| react-pi-message-projection › react-pi: streaming tail projection › 5000 stable messages | 30.32µs | +17.8% |  | 25.29µs | 48.04µs | 9 |
| sse-fragmentation › assistant-stream: fragmented SSE events › 100 KiB, 1 chunks | 6.29µs | +33.4% |  | 4.70µs | 7.35µs | 9 |
| sse-fragmentation › assistant-stream: fragmented SSE events › 100 KiB, 101 chunks | 17.73µs | +13.5% |  | 15.35µs | 24.21µs | 9 |
| sse-fragmentation › assistant-stream: fragmented SSE events › 1024 KiB, 1 chunks | 60.61µs | +31.8% |  | 45.83µs | 72.66µs | 9 |
| sse-fragmentation › assistant-stream: fragmented SSE events › 1024 KiB, 1025 chunks | 209.43µs | +8.3% |  | 183.03µs | 344.23µs | 9 |
| thread-scaling › external-store thread: mount+unmount by message count › 10 messages | 5.130ms | +12.2% |  | 3.941ms | 6.950ms | 9 |
| thread-scaling › external-store thread: mount+unmount by message count › 100 messages | 27.924ms | +0.4% |  | 22.883ms | 45.070ms | 9 |
| thread-scaling › external-store thread: mount+unmount by message count › 1000 messages | 329.334ms | +2.7% |  | 303.432ms | 471.630ms | 9 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › 20 message window, 10 messages | 415.63µs | +2.0% |  | 329.18µs | 626.18µs | 9 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › 20 message window, 100 messages | 706.03µs | +10.0% |  | 635.87µs | 946.59µs | 9 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › 20 message window, 1000 messages | 3.809ms | +21.4% |  | 2.761ms | 4.653ms | 9 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › all messages by id, 10 messages | 466.18µs | +14.2% |  | 336.50µs | 635.03µs | 9 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › all messages by id, 100 messages | 1.315ms | +17.4% |  | 1.079ms | 1.674ms | 9 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › all messages by id, 1000 messages | 9.320ms | +14.0% |  | 8.034ms | 15.272ms | 9 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › all messages, 10 messages | 393.62µs | +14.0% |  | 311.25µs | 667.45µs | 9 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › all messages, 100 messages | 942.03µs | +12.1% |  | 781.80µs | 1.197ms | 9 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › all messages, 1000 messages | 6.277ms | +15.9% |  | 5.241ms | 9.906ms | 9 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › provider only, 10 messages | 186.75µs | +15.7% |  | 145.04µs | 333.61µs | 9 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › provider only, 100 messages | 399.61µs | +10.8% |  | 359.63µs | 544.61µs | 9 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › provider only, 1000 messages | 2.743ms | +2.9% |  | 2.329ms | 3.392ms | 9 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › runtime only, 10 messages | 13.20µs | +17.3% |  | 10.93µs | 25.72µs | 9 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › runtime only, 100 messages | 26.83µs | +18.4% |  | 22.08µs | 40.73µs | 9 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › runtime only, 1000 messages | 234.57µs | +19.3% |  | 183.75µs | 306.29µs | 9 |
| thread-scaling › external-store thread: one token changed in the last message, by thread length › 10 messages | 488.83µs | +24.6% |  | 392.19µs | 714.62µs | 9 |
| thread-scaling › external-store thread: one token changed in the last message, by thread length › 100 messages | 1.011ms | +18.2% |  | 810.46µs | 1.238ms | 9 |
| thread-scaling › external-store thread: one token changed in the last message, by thread length › 1000 messages | 6.316ms | +4.8% |  | 5.162ms | 10.929ms | 9 |
| tool-args › assistant-stream: accumulator tool arguments (16-char deltas) › 1000 bytes | 202.85µs | +24.8% |  | 156.10µs | 273.57µs | 9 |
| tool-args › assistant-stream: accumulator tool arguments (16-char deltas) › 10000 bytes | 1.843ms | +25.0% |  | 1.447ms | 2.358ms | 9 |
| tool-args › assistant-stream: accumulator tool arguments (16-char deltas) › 5000 bytes | 913.89µs | +22.1% |  | 724.66µs | 1.191ms | 9 |
| tool-args › assistant-stream: active-reader tool arguments (16-char deltas) › 1000 bytes | 233.28µs | +28.4% |  | 175.27µs | 318.76µs | 9 |
| tool-args › assistant-stream: active-reader tool arguments (16-char deltas) › 10000 bytes | 2.049ms | +29.6% |  | 1.522ms | 2.684ms | 9 |
| tool-args › assistant-stream: active-reader tool arguments (16-char deltas) › 5000 bytes | 1.022ms | +27.7% |  | 784.09µs | 1.366ms | 9 |
| tool-args › assistant-stream: complete accumulated arguments (single delta) › 10,000 array elements | 311.90µs | +26.3% |  | 245.47µs | 346.51µs | 9 |
| tool-args › assistant-stream: dense accumulated arguments (16-char deltas) › 2,000 array entries | 19.299ms | +12.5% |  | 16.472ms | 26.611ms | 9 |
| tool-args › assistant-stream: dense accumulated arguments (16-char deltas) › 2,000 object entries | 755.230ms | +13.4% |  | 461.969ms | 850.924ms | 9 |
| tool-args › assistant-stream: execute-only tool arguments (16-char deltas) › 1000 bytes | 170.94µs | +31.5% |  | 127.23µs | 237.05µs | 9 |
| tool-args › assistant-stream: execute-only tool arguments (16-char deltas) › 10000 bytes | 1.379ms | +26.6% |  | 1.052ms | 1.901ms | 9 |
| tool-args › assistant-stream: execute-only tool arguments (16-char deltas) › 5000 bytes | 697.64µs | +28.7% |  | 534.39µs | 976.37µs | 9 |
| tool-args › assistant-stream: long string arguments (4096-char deltas) › accumulator: 10000 bytes | 177.13µs | +22.7% |  | 144.39µs | 210.61µs | 9 |
| tool-args › assistant-stream: long string arguments (4096-char deltas) › accumulator: 50000 bytes | 846.06µs | +23.2% |  | 686.60µs | 980.26µs | 9 |
| tool-args › assistant-stream: long string arguments (4096-char deltas) › active-reader: 10000 bytes | 192.72µs | +23.7% |  | 155.74µs | 231.11µs | 9 |
| tool-args › assistant-stream: long string arguments (4096-char deltas) › active-reader: 50000 bytes | 870.38µs | +21.4% |  | 716.23µs | 1.020ms | 9 |
| tree › tree mount+unmount, 500 leaves x 10 hooks › createTapRoot | 2.899ms | +26.6% |  | 2.256ms | 3.714ms | 9 |
| tree › tree mount+unmount, 500 leaves x 10 hooks › createTapRootDeps | 2.749ms | +15.3% |  | 2.288ms | 3.717ms | 9 |
| tree › tree mount+unmount, 500 leaves x 10 hooks › createTapRootStable | 2.720ms | +18.1% |  | 2.221ms | 3.698ms | 9 |
| tree › tree mount+unmount, 500 leaves x 10 hooks › react | 2.895ms | +33.6% |  | 2.150ms | 3.726ms | 9 |
| tree › tree mount+unmount, 500 leaves x 10 hooks › tapRoot | 1.853ms | +21.9% |  | 1.405ms | 2.350ms | 9 |
| tree › tree update: one leaf dispatch, 500 leaves x 10 hooks › createTapRoot | 2.746ms | +26.1% |  | 2.161ms | 3.512ms | 9 |
| tree › tree update: one leaf dispatch, 500 leaves x 10 hooks › createTapRootDeps | 2.662ms | +20.3% |  | 2.179ms | 3.507ms | 9 |
| tree › tree update: one leaf dispatch, 500 leaves x 10 hooks › createTapRootStable | 182.73µs | -17.2% |  | 166.62µs | 305.20µs | 9 |
| tree › tree update: one leaf dispatch, 500 leaves x 10 hooks › react | 109.66µs | +15.2% |  | 94.44µs | 148.10µs | 9 |
| tree › tree update: one leaf dispatch, 500 leaves x 10 hooks › tapRoot | 1.434ms | +26.6% |  | 1.108ms | 1.825ms | 9 |
| useResources › useResources mount+unmount, 500 children x 10 hooks › deps | 1.484ms | +20.0% |  | 1.185ms | 2.116ms | 9 |
| useResources › useResources mount+unmount, 500 children x 10 hooks › no-deps | 1.617ms | +21.5% |  | 1.294ms | 2.162ms | 9 |
| useResources › useResources: one child dispatch, 500 children x 10 hooks › deps | 36.85µs | +23.3% |  | 29.71µs | 54.18µs | 9 |
| useResources › useResources: one child dispatch, 500 children x 10 hooks › no-deps | 39.35µs | +21.1% |  | 31.55µs | 54.70µs | 9 |
| useResources › useResources: rebuild elements array, 500 children x 10 hooks › deps | 55.02µs | +17.8% |  | 45.20µs | 72.42µs | 9 |
| useResources › useResources: rebuild elements array, 500 children x 10 hooks › no-deps | 1.311ms | +23.5% |  | 990.30µs | 1.600ms | 9 |

informational; points come from different runners of the same class, so read trends, not single deltas.
