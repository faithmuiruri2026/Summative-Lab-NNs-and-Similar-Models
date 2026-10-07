# Notes Observed.

- `` If you don't have patient to wait,``  don't uncomment this  ``REALWASTE_URL `` since it will erase the existing dataset and download new one.

- **Changed RAG generation to include validation and fallback handling.**
Replaced the basic `rag_answer()` pipeline with `rag_answer_checked()`, which validates the fine-tuned model's generated response against the retrieved policy context and falls back to the authoritative policy sections when hard faithfulness issues are detected.
