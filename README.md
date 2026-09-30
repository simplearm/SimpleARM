# SimpleARM: Simple Agentic Memory for Generalist Robot Policies

[![Project Page](https://img.shields.io/badge/Project-Page-111827?style=flat-square)](https://simplearm.github.io)
[![arXiv](https://img.shields.io/badge/arXiv-2609.36595-b31b1b?style=flat-square)](https://arxiv.org/abs/2609.36595)

Yuyou Zhang<sup>1,*</sup>, Yunbei Zhang<sup>2,*</sup>, Miao Li<sup>1</sup>, Janet Wang<sup>2</sup>, Zijian Jin<sup>3</sup>, Shilong Liu<sup>4,5</sup>, Ding Zhao<sup>1</sup>

<sup>1</sup>Carnegie Mellon University · <sup>2</sup>Tulane University · <sup>3</sup>New York University · <sup>4</sup>Princeton University · <sup>5</sup>Columbia University

<sup>*</sup>Equal contribution

**Code will be released soon.**

## Abstract

Visual-memory systems commonly retain or compress past observations. Robot control additionally requires interaction-derived state that no individual frame may explicitly represent, such as persistent identity relations, accumulated progress, or ordered procedures. We introduce *Simple Agentic Robot Memory* (**SimpleARM**), a training-free memory layer for frozen generalist robot policies. From the task instruction, SimpleARM specifies what to monitor; frozen perceptual tools maintain compact typed state online; structured access retrieves that state only when a proposed subgoal depends on history; and current-view grounding resolves recalled entities before execution. We evaluate SimpleARM on RoboMME, a benchmark of memory-dependent robot manipulation tasks that require history information no longer available in the current observation. Across all 16 tasks and three policy seeds, SimpleARM achieves **67.17%** mean success, compared with **44.51%** for the strongest non-oracle baseline. Matched ablations show mechanism specificity: removing relation, reference, progress, or route state produces large losses where the affected state is retrieved for control, while largely sparing other tasks. These results support a state-based view of robot memory: effective memory for control is not simply retained visual history, but compact task-relevant state derived from the interaction history.

## Citation

If you find SimpleARM useful, please cite our [paper](https://arxiv.org/abs/2609.36595):

```bibtex
@misc{zhang2026simpleagenticmemorygeneralist,
  title={Simple Agentic Memory for Generalist Robot Policies},
  author={Yuyou Zhang and Yunbei Zhang and Miao Li and Janet Wang and Zijian Jin and Shilong Liu and Ding Zhao},
  year={2026},
  eprint={2609.36595},
  archivePrefix={arXiv},
  primaryClass={cs.RO},
  url={https://arxiv.org/abs/2609.36595},
}
```
