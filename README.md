# Custom Fields Documentation

Documentation for the Filament Custom Fields plugin, supporting both v1 and v2 versions.

## Structure

```
.
├── v1/                 # Version 1 specific documentation
│   ├── introduction.mdx
│   ├── installation.mdx
│   ├── quickstart.mdx
│   └── essentials/     # v1 configuration and features
├── v2/                 # Version 2 specific documentation
│   ├── introduction.mdx  # v2 features and improvements
│   ├── installation.mdx  # v2 installation guide
│   ├── quickstart.mdx
│   ├── upgrade.mdx       # v1 to v2 upgrade guide
│   └── essentials/       # v2 configuration and features
├── help-support/       # Help and support documentation
│   ├── support.mdx       # Support information
│   └── contributing.mdx  # Contribution guide
├── legal-acknowledgments/ # Legal and licensing documentation
│   ├── license.mdx       # Licensing information
│   └── code-distribution.mdx # Code distribution info
├── images/             # Shared images
├── logo/               # Logo files
└── docs.json           # Mintlify configuration with versioning
```

## Version Management

The documentation uses Mintlify's built-in versioning system:

- **Default version**: v2 (latest)
- **Supported versions**: v1, v2
- **Version switcher**: Automatically available in the documentation UI

## Key Differences Between Versions

### Version 1
- Original implementation
- Basic field types
- Standard caching
- Laravel 10+ / Filament 3+ support

### Version 2
- Enhanced performance (50% faster rendering)
- New field types (JSON, Rich Editor, Code Editor)
- Improved validation with custom rule builders
- Better UI/UX with drag-and-drop ordering
- TypeScript support
- Laravel 12+ / Filament 4+ support
- Backward compatible upgrade path

## Upgrade Documentation

Users can find upgrade instructions at `/v2/upgrade` which includes:
- Automatic upgrade command
- Manual upgrade steps
- Breaking changes
- Rollback procedures

## Shared Documentation

The `/shared` directory contains documentation that applies to all versions:
- Core concepts
- General best practices
- Architecture overview

## Local Development

To run the documentation locally:

```bash
npx mintlify dev
```

## Deployment

The documentation is automatically deployed when pushing to the main branch.

## Contributing

When adding new documentation:
1. Determine if it's version-specific or shared
2. Place in appropriate directory (v1/, v2/, help-support/, or legal-acknowledgments/)
3. Update docs.json navigation if adding new pages
4. Ensure version-specific features are clearly marked