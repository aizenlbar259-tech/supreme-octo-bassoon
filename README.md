space-shooter-js/
├── public/
│   ├── index.html               # Entry point (with responsive viewport)
│   ├── assets/
│   │   ├── textures/            # Optimized sprites/textures
│   │   │   ├── ships/
│   │   │   ├── projectiles/
│   │   │   ├── backgrounds/     # Parallax + animated BGs
│   │   │   └── ui/
│   │   ├── audio/               # Spatial audio files
│   │   │   ├── sfx/
│   │   │   └── music/
│   │   └── shaders/             # Custom WebGL shaders
│   │       ├── starfield.glsl
│   │       └── explosion.glsl
│   ├── css/
│   │   ├── main.css             # Global styles + responsive rules
│   │   └── animations.css       # Keyframe + transition effects
│   └── js/
│       ├── main.js              # Entry point (uses ES modules)
│       ├── core/               # Game engine core
│       │   ├── Game.js         # State machine + loop
│       │   ├── Input.js        # Multi-input support (keyboard, touch, gamepad)
│       │   ├── Physics.js      # Matter.js integration
│       │   ├── Renderer.js     # Canvas + WebGL renderer
│       │   └── Audio.js        # Spatial audio + Howler.js
│       ├── entities/            # Modular game objects
│       │   ├── Player/         # Player ship module
│       │   │   ├── index.js
│       │   │   ├── Controls.js
│       │   │   └── Weapons.js
│       │   ├── Enemies/        # Enemy types with AI behaviors
│       │   │   ├── BasicEnemy.js
│       │   │   ├── EliteEnemy.js
│       │   │   └── BossEnemy.js
│       │   ├── Projectiles/
│       │   └── PowerUps/
│       ├── systems/             # Game systems
│       │   ├── Collision.js    # Broadphase + narrowphase detection
│       │   ├── Spawner.js      # Wave-based enemy spawning
│       │   ├── UI.js           # HUD + menus (Phaser-like UI)
│       │   └── SaveSystem.js   # LocalStorage + cloud sync
│       └── config/             # Environment-specific config
│           ├── gameSettings.js
│           └── assetPaths.js
├── package.json                 # Dependencies + scripts
├── webpack.config.js            # Bundling + optimization
├── README.md                    # Docs + contribution guide
└── LICENSE
