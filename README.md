# Make Your Avatar - Z-Image AI

Train a personalized AI model with your photos and create stunning avatars in any style using [fal.ai's Z-Image](https://fal.ai/models/fal-ai/z-image-trainer) model.

[![Powered by fal.ai](https://img.shields.io/badge/Powered%20by-fal.ai-06b6d4?style=for-the-badge&logo=data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMjQiIGhlaWdodD0iMjQiIHZpZXdCb3g9IjAgMCAyNCAyNCIgZmlsbD0ibm9uZSIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj48cGF0aCBkPSJNMTMgMTBWM0w0IDE0aDd2N2w5LTExaC03eiIgc3Ryb2tlPSJ3aGl0ZSIgc3Ryb2tlLXdpZHRoPSIyIiBzdHJva2UtbGluZWNhcD0icm91bmQiIHN0cm9rZS1saW5lam9pbj0icm91bmQiLz48L3N2Zz4=)](https://fal.ai/models/fal-ai/z-image/turbo/lora)

## Features

- **Upload Photos**: Drag & drop 5+ photos of yourself
- **Train Your Model**: Create a personalized LoRA model using Z-Image Trainer
- **Generate Avatars**: Create stunning images in any style
- **Save Models**: Store trained models in localStorage for later use
- **Modern UI**: Beautiful dark theme with glassmorphism effects and smooth animations

## Tech Stack

- **Next.js 14** - React framework with App Router
- **Tailwind CSS** - Utility-first CSS
- **Framer Motion** - Animation library
- **fal.ai** - AI inference APIs
- **JSZip** - Client-side zip creation

## Getting Started

### Prerequisites

- Node.js 18+ 
- A [fal.ai](https://fal.ai) account and API key

### Installation

1. Clone the repository:
```bash
git clone <your-repo-url>
cd makeyouravatar-zimage
```

2. Install dependencies:
```bash
npm install
```

3. Create a `.env.local` file in the root directory:
```env
FAL_KEY=your_fal_api_key_here
```

Get your FAL API key from: https://fal.ai/dashboard/keys

4. Run the development server:
```bash
npm run dev
```

5. Open [http://localhost:3000](http://localhost:3000) in your browser.

## Deployment on Railway

1. Push your code to GitHub
2. Connect your repository to [Railway](https://railway.app)
3. Add the `FAL_KEY` environment variable in Railway's settings
4. Deploy!

Railway will automatically detect the Next.js project and build it.

## Usage

### Step 1: Upload Photos
Upload at least 5 clear photos of yourself. The more diverse angles and lighting, the better your model will be.

### Step 2: Configure Training
- **Model Name**: Give your model a memorable name
- **Training Focus**: Choose between content (face focus), balanced, or style
- **Training Steps**: More steps = better quality but higher cost

### Step 3: Train
Wait for training to complete (typically 3-5 minutes). You can watch the progress in real-time.

### Step 4: Generate
Use prompts with "TOK person" to reference yourself:
- "TOK person as a superhero"
- "TOK person in a professional portrait"
- "TOK person as an anime character"


## API Reference

This project uses two fal.ai models:

- **[Z-Image Trainer](https://fal.ai/models/fal-ai/z-image-trainer/api)**: For LoRA training
- **[Z-Image Turbo with LoRA](https://fal.ai/models/fal-ai/z-image/turbo/lora/api)**: For image generation

## License

MIT
