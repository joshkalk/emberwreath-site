# Visual Component Classes

Use these reusable classes to keep images, cards, and tables consistent across Emberwreath player-facing pages.

## Images

- **Map or large content image:** wrap the image in `.image-frame`.
- **Species overview image:** use `.species-card-media` for the image container and `.species-card-image` on the image itself. Use this only for cropped species overview thumbnails.
- **Full species-page class or adventurer art:** wrap figures in `.species-art-grid` and apply `.species-art` to each figure so full PHB art remains contained without thumbnail cropping.
- **Island hero image:** wrap the image in `.hero-image`.
- **Reference sheet:** wrap the image in `.reference-image` so the full sheet remains visible without cropping.

## Tables

- **Responsive comparison table:** wrap the table in `.table-wrap` and apply `.comparison-table` to the table.

## Safety rule

Do not add unconstrained raw images to content pages. Every image should use a known component class or a new page-specific constrained class. Use `.species-card-media`/`.species-card-image` for overview thumbnails, `.species-art-grid`/`.species-art` for full species-page art, and `.reference-image` for uncropped reference sheets.
