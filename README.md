## aui-perf nightly record

_1 points · 2026-11-19T04:31:14.259Z to 2026-11-19T04:31:14.259Z · latest runner: Intel(R) Xeon(R) Platinum 8370C CPU @ 2.80GHz · Node v26.13.0_

| bench | latest | Δ7d | Δ30d | min | max | points |
| --- | ---: | ---: | ---: | ---: | ---: | ---: |
| accumulator › assistant-stream: raw controller enqueue overhead › 10,000 chunks from one source stream | 864.27µs |  |  | 864.27µs | 864.27µs | 1 |
| accumulator › assistant-stream: raw controller enqueue overhead › 10,000 controller.enqueue calls | 1.209ms |  |  | 1.209ms | 1.209ms | 1 |
| accumulator › assistant-stream: same 4000-char text, chunk size A/B › 16 deltas × 250 chars | 58.22µs |  |  | 58.22µs | 58.22µs | 1 |
| accumulator › assistant-stream: same 4000-char text, chunk size A/B › 250 deltas × 16 chars | 666.48µs |  |  | 666.48µs | 666.48µs | 1 |
| accumulator › assistant-stream: same 4000-char text, chunk size A/B › 4000 deltas × 1 char (per-token) | 10.380ms |  |  | 10.380ms | 10.380ms | 1 |
| accumulator › assistant-stream: stream + accumulator per-delta cost (16-char deltas) › 100 deltas | 282.75µs |  |  | 282.75µs | 282.75µs | 1 |
| accumulator › assistant-stream: stream + accumulator per-delta cost (16-char deltas) › 1000 deltas | 2.627ms |  |  | 2.627ms | 2.627ms | 1 |
| accumulator › assistant-stream: stream + accumulator per-delta cost (16-char deltas) › 4000 deltas | 10.360ms |  |  | 10.360ms | 10.360ms | 1 |
| accumulator › assistant-stream: stream round trip baseline, no accumulator › 100 deltas | 10.11µs |  |  | 10.11µs | 10.11µs | 1 |
| accumulator › assistant-stream: stream round trip baseline, no accumulator › 1000 deltas | 83.38µs |  |  | 83.38µs | 83.38µs | 1 |
| accumulator › assistant-stream: stream round trip baseline, no accumulator › 4000 deltas | 327.66µs |  |  | 327.66µs | 327.66µs | 1 |
| ai-sdk-system-metadata › ai-sdk: system-message metadata conversion through the runtime › 128 parts, distinct providers (stress) | 107.40µs |  |  | 107.40µs | 107.40µs | 1 |
| ai-sdk-system-metadata › ai-sdk: system-message metadata conversion through the runtime › 16 parts, one repeated provider | 65.03µs |  |  | 65.03µs | 65.03µs | 1 |
| ai-sdk-system-metadata › ai-sdk: system-message metadata conversion through the runtime › 2 parts, one repeated provider | 63.42µs |  |  | 63.42µs | 63.42µs | 1 |
| ai-sdk-system-metadata › ai-sdk: system-message metadata conversion through the runtime › 512 parts, distinct providers (stress) | 318.13µs |  |  | 318.13µs | 318.13µs | 1 |
| ai-sdk-toolkit › ai-sdk: convert fresh AISDKToolkit schemas › 10 static tools | 77.43µs |  |  | 77.43µs | 77.43µs | 1 |
| ai-sdk-toolkit › ai-sdk: convert fresh AISDKToolkit schemas › 100 static tools | 698.64µs |  |  | 698.64µs | 698.64µs | 1 |
| ai-sdk-toolkit › ai-sdk: reuse converted AISDKToolkit schemas › 10 static tools | 10.45µs |  |  | 10.45µs | 10.45µs | 1 |
| ai-sdk-toolkit › ai-sdk: reuse converted AISDKToolkit schemas › 100 static tools | 82.65µs |  |  | 82.65µs | 82.65µs | 1 |
| data-stream › assistant-stream: data stream decode (16-char deltas) › 100 deltas | 732.11µs |  |  | 732.11µs | 732.11µs | 1 |
| data-stream › assistant-stream: data stream decode (16-char deltas) › 1000 deltas | 5.932ms |  |  | 5.932ms | 5.932ms | 1 |
| data-stream › assistant-stream: data stream decode (16-char deltas) › 4000 deltas | 23.420ms |  |  | 23.420ms | 23.420ms | 1 |
| data-stream › assistant-stream: data stream encode (16-char deltas) › 100 deltas | 359.72µs |  |  | 359.72µs | 359.72µs | 1 |
| data-stream › assistant-stream: data stream encode (16-char deltas) › 1000 deltas | 3.455ms |  |  | 3.455ms | 3.455ms | 1 |
| data-stream › assistant-stream: data stream encode (16-char deltas) › 4000 deltas | 13.626ms |  |  | 13.626ms | 13.626ms | 1 |
| external-message-conversion › core: cached external message conversion, one streaming delta › 1000 messages, 6-part replies | 286.73µs |  |  | 286.73µs | 286.73µs | 1 |
| external-message-conversion › core: cached external message conversion, one streaming delta › 5000 messages, 20-part replies | 2.175ms |  |  | 2.175ms | 2.175ms | 1 |
| external-message-conversion › core: external message reasoning continuations › 100 matches | 69.92µs |  |  | 69.92µs | 69.92µs | 1 |
| external-message-conversion › core: external message reasoning continuations › 1000 matches | 710.18µs |  |  | 710.18µs | 710.18µs | 1 |
| external-message-conversion › core: external message reasoning continuations › 5000 matches | 3.843ms |  |  | 3.843ms | 3.843ms | 1 |
| external-message-conversion › core: external message tool results › 100 matches | 76.59µs |  |  | 76.59µs | 76.59µs | 1 |
| external-message-conversion › core: external message tool results › 1000 matches | 781.90µs |  |  | 781.90µs | 781.90µs | 1 |
| external-message-conversion › core: external message tool results › 5000 matches | 4.273ms |  |  | 4.273ms | 4.273ms | 1 |
| external-message-conversion › core: external message unique tool calls › 100 matches | 40.30µs |  |  | 40.30µs | 40.30µs | 1 |
| external-message-conversion › core: external message unique tool calls › 1000 matches | 396.22µs |  |  | 396.22µs | 396.22µs | 1 |
| external-message-conversion › core: external message unique tool calls › 5000 matches | 2.193ms |  |  | 2.193ms | 2.193ms | 1 |
| from-thread-message-like › core: fromThreadMessageLike text parts › 1 text parts | 0.27µs |  |  | 0.27µs | 0.27µs | 1 |
| from-thread-message-like › core: fromThreadMessageLike text parts › 10 text parts | 0.47µs |  |  | 0.47µs | 0.47µs | 1 |
| from-thread-message-like › core: fromThreadMessageLike text parts › 100 text parts | 2.47µs |  |  | 2.47µs | 2.47µs | 1 |
| from-thread-message-like › core: fromThreadMessageLike tool calls › 1 tool calls | 0.68µs |  |  | 0.68µs | 0.68µs | 1 |
| from-thread-message-like › core: fromThreadMessageLike tool calls › 10 tool calls | 3.51µs |  |  | 3.51µs | 3.51µs | 1 |
| from-thread-message-like › core: fromThreadMessageLike tool calls › 100 tool calls | 30.61µs |  |  | 30.61µs | 30.61µs | 1 |
| interactable-array-patches › core: id-keyed interactable array patches › 1000 items and patches | 150.94µs |  |  | 150.94µs | 150.94µs | 1 |
| interactable-array-patches › core: id-keyed interactable array patches › 5000 items and patches | 847.87µs |  |  | 847.87µs | 847.87µs | 1 |
| markdown-preprocess › react-markdown: preprocess › escapeCurrencyDollars, 20,000 tilde runs on one line | 2.735ms |  |  | 2.735ms | 2.735ms | 1 |
| markdown-preprocess › react-markdown: preprocess › escapeCurrencyDollars, 20,000 tildes after prose | 186.13µs |  |  | 186.13µs | 186.13µs | 1 |
| markdown-preprocess › react-markdown: preprocess › escapeCurrencyDollars, 20,000 triple-backtick spans on one line | 3.695ms |  |  | 3.695ms | 3.695ms | 1 |
| markdown-preprocess › react-markdown: preprocess › escapeCurrencyDollars, 5,000 code spans in one paragraph | 513.75µs |  |  | 513.75µs | 513.75µs | 1 |
| markdown-preprocess › react-markdown: preprocess › escapeCurrencyDollars, mixed message, 100 sections | 695.42µs |  |  | 695.42µs | 695.42µs | 1 |
| markdown-preprocess › react-markdown: preprocess › normalizeMathDelimiters, 20,000 tilde runs on one line | 7.351ms |  |  | 7.351ms | 7.351ms | 1 |
| markdown-preprocess › react-markdown: preprocess › normalizeMathDelimiters, 20,000 tildes after prose | 797.35µs |  |  | 797.35µs | 797.35µs | 1 |
| markdown-preprocess › react-markdown: preprocess › normalizeMathDelimiters, 20,000 triple-backtick spans on one line | 23.646ms |  |  | 23.646ms | 23.646ms | 1 |
| markdown-preprocess › react-markdown: preprocess › normalizeMathDelimiters, 5,000 code spans in one paragraph | 3.956ms |  |  | 3.956ms | 3.956ms | 1 |
| markdown-preprocess › react-markdown: preprocess › normalizeMathDelimiters, mixed message, 100 sections | 2.700ms |  |  | 2.700ms | 2.700ms | 1 |
| markdown-streaming › react-markdown: one token after an unchanged fenced code block › 10 KB fenced Markdown | 2.948ms |  |  | 2.948ms | 2.948ms | 1 |
| markdown-streaming › react-markdown: one token after an unchanged fenced code block › 10 KB fenced Markdown deferred | 3.215ms |  |  | 3.215ms | 3.215ms | 1 |
| markdown-streaming › react-markdown: one token after an unchanged fenced code block › 100 KB fenced Markdown | 20.559ms |  |  | 20.559ms | 20.559ms | 1 |
| markdown-streaming › react-markdown: one token after an unchanged fenced code block › 100 KB fenced Markdown deferred | 21.700ms |  |  | 21.700ms | 21.700ms | 1 |
| markdown-streaming › react-markdown: one token changed in the last paragraph, by message length › 1 paragraphs | 1.466ms |  |  | 1.466ms | 1.466ms | 1 |
| markdown-streaming › react-markdown: one token changed in the last paragraph, by message length › 10 paragraphs | 3.042ms |  |  | 3.042ms | 3.042ms | 1 |
| markdown-streaming › react-markdown: one token changed in the last paragraph, by message length › 50 paragraphs | 10.109ms |  |  | 10.109ms | 10.109ms | 1 |
| markdown-streaming › react-markdown: the same token with defer on › 1 paragraphs deferred | 1.187ms |  |  | 1.187ms | 1.187ms | 1 |
| markdown-streaming › react-markdown: the same token with defer on › 10 paragraphs deferred | 1.928ms |  |  | 1.928ms | 1.928ms | 1 |
| markdown-streaming › react-markdown: the same token with defer on › 50 paragraphs deferred | 4.642ms |  |  | 4.642ms | 4.642ms | 1 |
| react-langgraph › react-langgraph: streamed tool argument accumulation › 1000 character argument in 16-character deltas | 345.80µs |  |  | 345.80µs | 345.80µs | 1 |
| react-langgraph › react-langgraph: streamed tool argument accumulation › 10000 character argument in 16-character deltas | 2.851ms |  |  | 2.851ms | 2.851ms | 1 |
| react-langgraph › react-langgraph: streamed tool argument accumulation › 500 short object entries in 16-character deltas | 312.966ms |  |  | 312.966ms | 312.966ms | 1 |
| react-langgraph › react-langgraph: streamed tool argument accumulation › 50000 character argument in 16-character deltas | 13.543ms |  |  | 13.543ms | 13.543ms | 1 |
| react-pi-message-projection › react-pi: streaming tail projection › 10 stable messages | 2.32µs |  |  | 2.32µs | 2.32µs | 1 |
| react-pi-message-projection › react-pi: streaming tail projection › 1000 stable messages | 10.68µs |  |  | 10.68µs | 10.68µs | 1 |
| react-pi-message-projection › react-pi: streaming tail projection › 5000 stable messages | 48.04µs |  |  | 48.04µs | 48.04µs | 1 |
| sse-fragmentation › assistant-stream: fragmented SSE events › 100 KiB, 1 chunks | 5.99µs |  |  | 5.99µs | 5.99µs | 1 |
| sse-fragmentation › assistant-stream: fragmented SSE events › 100 KiB, 101 chunks | 24.21µs |  |  | 24.21µs | 24.21µs | 1 |
| sse-fragmentation › assistant-stream: fragmented SSE events › 1024 KiB, 1 chunks | 57.82µs |  |  | 57.82µs | 57.82µs | 1 |
| sse-fragmentation › assistant-stream: fragmented SSE events › 1024 KiB, 1025 chunks | 344.23µs |  |  | 344.23µs | 344.23µs | 1 |
| thread-scaling › external-store thread: mount+unmount by message count › 10 messages | 6.433ms |  |  | 6.433ms | 6.433ms | 1 |
| thread-scaling › external-store thread: mount+unmount by message count › 100 messages | 40.123ms |  |  | 40.123ms | 40.123ms | 1 |
| thread-scaling › external-store thread: mount+unmount by message count › 1000 messages | 435.602ms |  |  | 435.602ms | 435.602ms | 1 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › 20 message window, 10 messages | 626.18µs |  |  | 626.18µs | 626.18µs | 1 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › 20 message window, 100 messages | 934.98µs |  |  | 934.98µs | 934.98µs | 1 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › 20 message window, 1000 messages | 4.653ms |  |  | 4.653ms | 4.653ms | 1 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › all messages by id, 10 messages | 604.87µs |  |  | 604.87µs | 604.87µs | 1 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › all messages by id, 100 messages | 1.674ms |  |  | 1.674ms | 1.674ms | 1 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › all messages by id, 1000 messages | 15.272ms |  |  | 15.272ms | 15.272ms | 1 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › all messages, 10 messages | 667.45µs |  |  | 667.45µs | 667.45µs | 1 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › all messages, 100 messages | 1.197ms |  |  | 1.197ms | 1.197ms | 1 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › all messages, 1000 messages | 9.906ms |  |  | 9.906ms | 9.906ms | 1 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › provider only, 10 messages | 328.33µs |  |  | 328.33µs | 328.33µs | 1 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › provider only, 100 messages | 536.18µs |  |  | 536.18µs | 536.18µs | 1 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › provider only, 1000 messages | 3.392ms |  |  | 3.392ms | 3.392ms | 1 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › runtime only, 10 messages | 19.92µs |  |  | 19.92µs | 19.92µs | 1 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › runtime only, 100 messages | 34.55µs |  |  | 34.55µs | 34.55µs | 1 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › runtime only, 1000 messages | 306.29µs |  |  | 306.29µs | 306.29µs | 1 |
| thread-scaling › external-store thread: one token changed in the last message, by thread length › 10 messages | 680.34µs |  |  | 680.34µs | 680.34µs | 1 |
| thread-scaling › external-store thread: one token changed in the last message, by thread length › 100 messages | 1.238ms |  |  | 1.238ms | 1.238ms | 1 |
| thread-scaling › external-store thread: one token changed in the last message, by thread length › 1000 messages | 10.929ms |  |  | 10.929ms | 10.929ms | 1 |
| tool-args › assistant-stream: accumulator tool arguments (16-char deltas) › 1000 bytes | 273.57µs |  |  | 273.57µs | 273.57µs | 1 |
| tool-args › assistant-stream: accumulator tool arguments (16-char deltas) › 10000 bytes | 2.358ms |  |  | 2.358ms | 2.358ms | 1 |
| tool-args › assistant-stream: accumulator tool arguments (16-char deltas) › 5000 bytes | 1.191ms |  |  | 1.191ms | 1.191ms | 1 |
| tool-args › assistant-stream: active-reader tool arguments (16-char deltas) › 1000 bytes | 317.41µs |  |  | 317.41µs | 317.41µs | 1 |
| tool-args › assistant-stream: active-reader tool arguments (16-char deltas) › 10000 bytes | 2.684ms |  |  | 2.684ms | 2.684ms | 1 |
| tool-args › assistant-stream: active-reader tool arguments (16-char deltas) › 5000 bytes | 1.366ms |  |  | 1.366ms | 1.366ms | 1 |
| tool-args › assistant-stream: complete accumulated arguments (single delta) › 10,000 array elements | 342.19µs |  |  | 342.19µs | 342.19µs | 1 |
| tool-args › assistant-stream: dense accumulated arguments (16-char deltas) › 2,000 array entries | 25.892ms |  |  | 25.892ms | 25.892ms | 1 |
| tool-args › assistant-stream: dense accumulated arguments (16-char deltas) › 2,000 object entries | 810.818ms |  |  | 810.818ms | 810.818ms | 1 |
| tool-args › assistant-stream: execute-only tool arguments (16-char deltas) › 1000 bytes | 233.49µs |  |  | 233.49µs | 233.49µs | 1 |
| tool-args › assistant-stream: execute-only tool arguments (16-char deltas) › 10000 bytes | 1.901ms |  |  | 1.901ms | 1.901ms | 1 |
| tool-args › assistant-stream: execute-only tool arguments (16-char deltas) › 5000 bytes | 976.37µs |  |  | 976.37µs | 976.37µs | 1 |
| tool-args › assistant-stream: long string arguments (4096-char deltas) › accumulator: 10000 bytes | 203.22µs |  |  | 203.22µs | 203.22µs | 1 |
| tool-args › assistant-stream: long string arguments (4096-char deltas) › accumulator: 50000 bytes | 967.42µs |  |  | 967.42µs | 967.42µs | 1 |
| tool-args › assistant-stream: long string arguments (4096-char deltas) › active-reader: 10000 bytes | 224.65µs |  |  | 224.65µs | 224.65µs | 1 |
| tool-args › assistant-stream: long string arguments (4096-char deltas) › active-reader: 50000 bytes | 1.005ms |  |  | 1.005ms | 1.005ms | 1 |
| tree › tree mount+unmount, 500 leaves x 10 hooks › createTapRoot | 3.714ms |  |  | 3.714ms | 3.714ms | 1 |
| tree › tree mount+unmount, 500 leaves x 10 hooks › createTapRootDeps | 3.717ms |  |  | 3.717ms | 3.717ms | 1 |
| tree › tree mount+unmount, 500 leaves x 10 hooks › createTapRootStable | 3.698ms |  |  | 3.698ms | 3.698ms | 1 |
| tree › tree mount+unmount, 500 leaves x 10 hooks › react | 3.712ms |  |  | 3.712ms | 3.712ms | 1 |
| tree › tree mount+unmount, 500 leaves x 10 hooks › tapRoot | 2.350ms |  |  | 2.350ms | 2.350ms | 1 |
| tree › tree update: one leaf dispatch, 500 leaves x 10 hooks › createTapRoot | 3.512ms |  |  | 3.512ms | 3.512ms | 1 |
| tree › tree update: one leaf dispatch, 500 leaves x 10 hooks › createTapRootDeps | 3.507ms |  |  | 3.507ms | 3.507ms | 1 |
| tree › tree update: one leaf dispatch, 500 leaves x 10 hooks › createTapRootStable | 305.20µs |  |  | 305.20µs | 305.20µs | 1 |
| tree › tree update: one leaf dispatch, 500 leaves x 10 hooks › react | 118.29µs |  |  | 118.29µs | 118.29µs | 1 |
| tree › tree update: one leaf dispatch, 500 leaves x 10 hooks › tapRoot | 1.825ms |  |  | 1.825ms | 1.825ms | 1 |
| useResources › useResources mount+unmount, 500 children x 10 hooks › deps | 2.116ms |  |  | 2.116ms | 2.116ms | 1 |
| useResources › useResources mount+unmount, 500 children x 10 hooks › no-deps | 2.162ms |  |  | 2.162ms | 2.162ms | 1 |
| useResources › useResources: one child dispatch, 500 children x 10 hooks › deps | 47.23µs |  |  | 47.23µs | 47.23µs | 1 |
| useResources › useResources: one child dispatch, 500 children x 10 hooks › no-deps | 49.43µs |  |  | 49.43µs | 49.43µs | 1 |
| useResources › useResources: rebuild elements array, 500 children x 10 hooks › deps | 72.42µs |  |  | 72.42µs | 72.42µs | 1 |
| useResources › useResources: rebuild elements array, 500 children x 10 hooks › no-deps | 1.600ms |  |  | 1.600ms | 1.600ms | 1 |

informational; points come from different runners of the same class, so read trends, not single deltas.
