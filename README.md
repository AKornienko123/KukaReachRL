# KukaReachRL (Spring 2025 Project)

This project implements reinforcement learning (SAC, PPO, TD3) for a 7-DoF KUKA iiwa reach task using the PyBullet simulator. The agent learns to move the robot's end-effector to a random 3D target position.

---

## 📁 Structure


---

## 🧠 Algorithms

- ✅ **PID baseline**  
- ✅ **SAC** (vanilla, vectorized)  
- ✅ **PPO** (large-batch, on-policy)  
- ✅ **TD3**  
- ✅ **Optuna-SAC** (hyperparameter tuning)

---

## 🧪 Evaluation

- **Success threshold**: 5 cm  
- **Metrics**:
  - Final distance to target (lower is better)
  - Success rate (episodes with distance < 0.05 m)
  - Episode length (steps)
  - FPS (frames per second)
- **Saliency analysis**: visualized input importance for Optuna-SAC

---

## 📷 Media

See `artifacts/` for:
- 📊 GIFs of agent performance (front/back/left/top)
- 📈 Training reward logs (`TensorBoard` format)
- 🧠 Saliency barplots

---

## ⚙️ Training Configs

YAML files in `configs/` define:
- Physics parameters (gravity, time step)
- Reward shaping
- Curriculum thresholds
- Action discretization

---

## 🚀 Run in Colab

The project was trained on **Google Colab Pro** with:
- GPU: NVIDIA L4 (23 GB)
- CUDA: 12.5
- PyTorch: 2.6.0

To reproduce, upload notebook and configs to Colab and run all cells.

---


