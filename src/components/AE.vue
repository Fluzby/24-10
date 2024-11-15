<template>
    <div class="min-h-screen bg-gradient-to-b from-black to-purple p-8">
      <div class="max-w-6xl mx-auto">
        <!-- Hero Section -->
        <div class="text-center mb-16">
          <h1 class="text-5xl font-bold text-white mb-4">Adobe After Effects</h1>
          <p class="text-xl text-purple-200">Industry Standard Motion Graphics & Visual Effects</p>
        </div>
  
        <!-- Features Grid -->
        <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8">
          <div v-for="feature in features" 
               :key="feature.title"
               class="rounded-lg p-6 transform hover:scale-105 transition-transform duration-300">
            <div class="text-purple-400 text-4xl mb-4">
              <i :class="feature.icon"></i>
            </div>
            <h3 class="text-xl font-semibold text-white mb-2">{{ feature.title }}</h3>
            <p class="text-purple-200">{{ feature.description }}</p>
          </div>
        </div>
      </div>
    </div>
  </template>
  
  <script>
  export default {
    name: 'AfterEffectsFeatures',
    data() {
      return {
        features: [
          {
            title: 'Motion Graphics',
            icon: 'fas fa-video',
            description: 'Create stunning animations and title sequences with powerful motion graphics tools.'
          },
          {
            title: 'Visual Effects',
            icon: 'fas fa-magic',
            description: 'Add spectacular visual effects and compositing to your videos.'
          },
          {
            title: 'Animation',
            icon: 'fas fa-film',
            description: 'Bring your ideas to life with keyframe animation and motion tracking.'
          },
          {
            title: '3D Integration',
            icon: 'fas fa-cube',
            description: 'Seamlessly integrate 3D elements with Cinema 4D integration.'
          },
          {
            title: 'Templates',
            icon: 'fas fa-copy',
            description: 'Access thousands of pre-made templates to speed up your workflow.'
          },
          {
            title: 'Plugins',
            icon: 'fas fa-puzzle-piece',
            description: 'Extend functionality with third-party plugins and scripts.'
          }
        ],
        layers: [
          'Background',
          'Text Layer',
          'Effects',
          'Animation',
          'Overlay'
        ],
        exportFormats: [
          'MP4 (H.264)',
          'QuickTime',
          'GIF',
          'PNG Sequence',
          'ProRes',
          'Media Encoder Integration'
        ],
        requirements: [
          'Windows 10/11 or macOS',
          '16GB RAM (32GB recommended)',
          'GPU with 2GB VRAM',
          'SSD Storage',
          'Multi-core processor'
        ]
      }
    }
  }
  </script>