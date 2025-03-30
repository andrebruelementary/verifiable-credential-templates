# Verifiable Credential Templates

This repository hosts a collection of standardized templates for Decentralized Identifier (DID) Verifiable Credentials. These templates are designed to be used across various DID implementations, with a focus on interoperability and reuse.

## Repository Structure

Templates are organized into categories, each in its own directory:

```
/
├── education/
│   ├── university-diploma.json
│   └── course-certificate.json
├── professional/
│   ├── employment-verification.json
│   └── professional-license.json
├── identity/
│   ├── basic-id.json
│   └── membership.json
├── events/
│   ├── event-ticket.json
│   └── subscription.json
└── financial/
    ├── payment-proof.json
    └── insurance-proof.json
```

## Template Format

Each template follows a standard JSON format:

```json
{
  "id": "unique-template-id",
  "name": "Human-Readable Template Name",
  "description": "Detailed description of what this credential represents",
  "properties": [
    {
      "id": "property-id",
      "label": "Property Label",
      "type": "text|date|number|etc",
      "required": true|false
    },
    // Additional properties...
  ],
  "isPublic": true,
  "source": "identus"
}
```

## Relationship with Credential Builder Demo

This template repository works in conjunction with the [Credential Builder Demo](https://github.com/andrebruelementary/credential-builder-demo) project, which provides a browser extension demonstrating how these templates can be implemented in a user interface.

### How They Work Together

1. The Credential Builder Demo loads templates from this repository
2. Users can select templates to create verifiable credentials
3. Private templates can be saved locally within the extension
4. Users can suggest new templates for inclusion in this public repository

We encourage developers to build their own implementations using these templates, contributing to a growing ecosystem of interoperable credential solutions.

## Why Another Template Repository?

While the W3C maintains official examples and standards for Verifiable Credentials, this repository aims to provide:

1. **Greater Agility**: Templates can be added and updated more quickly
2. **Community Focus**: Catering specifically to the needs of the Cardano Identus community
3. **Practical Implementation**: Templates that have been tested in real-world applications
4. **Developer Friendly**: Designed for easy integration with existing projects

Our goal is to complement, not replace, the W3C standards while providing more flexibility and community-driven development.

## Contributing

### Suggesting Templates

To suggest a new template for inclusion in this repository:

1. Create a private template in the Credential Builder Demo
2. Click "Suggest Selected Template for Public Repository"
3. Complete the GitHub issue with any additional information
4. Maintainers will review and add approved templates

### Direct Contributions

You can also contribute directly through pull requests:

1. Fork this repository
2. Add your template(s) following the established format and directory structure
3. Submit a pull request with a clear description of the template's purpose and use cases

### Guidelines for Good Templates

- Use clear, descriptive property names
- Include comprehensive descriptions
- Follow existing patterns for similar credential types
- Consider internationalization needs
- Focus on reusability across different systems

## Repository Governance

This repository is currently maintained by [Elementary Software](https://github.com/andrebruelementary), but we welcome broader community involvement.

### Joining as a Maintainer

Representatives from DID products in the Cardano Identus community who wish to join as maintainers can:

1. Open an issue expressing interest
2. Include information about your organization/project
3. Describe how you plan to contribute

We're actively seeking to expand the group of maintainers to ensure this repository serves the broader DID community.

## License

All templates in this repository are available under the [MIT License](LICENSE), allowing for free use, modification, and distribution in both commercial and non-commercial applications.

---

For questions or discussions about this repository, please [open an issue](https://github.com/andrebruelementary/verifiable-credential-templates/issues/new) or contact the maintainers directly.
