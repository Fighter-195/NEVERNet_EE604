# NEVERNet: Neural Enhanced Vision for Effective Reflection Removal

Implementation of our IIT Kanpur course project **“NEVERNet: Neural Enhanced Vision for Effective Reflection Removal”**,  
an enhanced version of ERRNet focusing on architectural and data-level refinements to improve reflection suppression and photometric consistency.

---

## Highlights

- Introduces a **hybrid activation design** combining *shifted tanh* and *Leaky ReLU* for smoother, stable gradient learning.
- Includes a **custom-built reflection detection module** (written from scratch) to identify reflection-dominant regions before main model inference.  
- Explores **RAW image-based inputs**, inspired by Adobe’s image formation study, to maintain linear color and brightness information.  
- Proposes a **DSLR + polarizing filter** method for simplified reflection/non-reflection dataset creation.  
- Provides an interactive **Gradio-based UI** for visualization and testing.

Example result of reflection detection and removal:
<p align="center">
  <img src="results/sample_input.jpg" width="250">
  <img src="results/reflection_mask.jpg" width="250">
  <img src="results/output_cleaned.jpg" width="250">
</p>

---

## Prerequisites

- **Python:** ≥ 3.8  
- **PyTorch:** ≥ 1.8  
- **Dependencies:** `opencv-python`, `numpy`, `matplotlib`, `gradio`, `torchvision`
- **Recommended Platform:** Ubuntu 22.04   
- **Hardware:** GPU optional (tested on NVIDIA RTX 4060)

Install all dependencies:
`
pip install -r requirements.txt

