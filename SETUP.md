# Setup

1. Create a **public** repository named exactly `sakib-18`.
2. Copy this package into that repository.
3. Replace `YOUR_LINKEDIN_URL`, `YOUR_EMAIL`, and `YOUR_REPOSITORY_LINK` in `README.md`.
4. In GitHub: **Settings → Actions → General** and allow Actions.
5. Set workflow permissions to allow workflows to write repository contents.
6. Run both workflows manually once:
   - **Generate Contribution Snake**
   - **Generate 3D Contribution Profile**
7. After they succeed, return to the profile page.

Expected structure:

sakib-18/
├── README.md
├── assets/hero.svg
├── scripts/generate_profile_asset.py
└── .github/workflows/
    ├── snake.yml
    └── profile-3d.yml

The main hero is local, so the profile's visual identity does not depend on a third-party stats service.

To regenerate the hero after editing the Python script:

```bash
python scripts/generate_profile_asset.py
```
