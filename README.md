# Halloween

A novel book project.

## Project Structure

```
halloween/
  content/          # AI-generated chapters (via booker write)
  outline/          # AI-generated book outline
  chapter_outlines/ # AI-generated detailed chapter outlines
  narrative_constants/ # Story Bible (characters, locations, style guide)
  assets/
    images/         # Generated artwork
    metadata/       # AI-generated metadata
  dist/             # Built ePub files
  config.yaml       # Book configuration
```

## Workflow

1. **Generate outline**: `booker outline "Halloween" --description "Your book description"`
2. **Generate story Bible**: `booker assets "Halloween"`
3. **Generate chapter outlines**: `booker chapter "Halloween" --all`
4. **Write chapters**: `booker write "Halloween" --all`
5. **Generate artwork**: `booker artwork config.yaml --use-claude`
6. **Build ePub**: `booker epub config.yaml`

## Configuration

Edit `config.yaml` to customize:
- Book metadata (title, author, description)
- AI models per task (Haiku/Sonnet/Opus)
- Chapter structure
- Styling and fonts
- Artwork settings

## Commands

```bash
# Generate AI outline
booker outline "Halloween" --description "Your book description" --chapters 10

# Generate story Bible (characters, locations, style guide, continuity)
booker assets "Halloween"

# Generate detailed chapter outlines
booker chapter "Halloween" --all

# Write chapters with AI
booker write "Halloween" --all --words 3500

# Generate artwork
booker artwork config.yaml --use-claude --formats epub

# Build ePub
booker epub config.yaml
```

## Template

This project uses the `novel` book type.

See `docs/TEMPLATES.md` and `docs/BOOK_STYLES.md` for documentation.
