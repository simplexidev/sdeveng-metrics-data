# SimplexiDev Engineering Toolkit Metrics Data

Reviewed, sanitized, versioned evaluation aggregates for
[`simplexidev/sdeveng`](https://github.com/simplexidev/sdeveng).

- `public/` contains publishable aggregates and the explicit publication manifest.
- `private/` contains only the policy for ignored local staging; raw material is never
  committed.

Schemas and validators live in
[`sdeveng-metrics-tooling`](https://github.com/simplexidev/sdeveng-metrics-tooling).
The approved data is presented by
[`sdeveng-metrics-dashboard`](https://github.com/simplexidev/sdeveng-metrics-dashboard).

The versioned dashboard interface is `public/publication-manifest.json` (schema `1.0`)
plus its listed sanitized JSON artifacts. Validate with explicit repository paths:

```console
dotnet run --project ../sdeveng-metrics-tooling/src/SdevEng.Metrics -- \
  publish-pages <dashboard-directory> public _site
```

## License

MIT. See [LICENSE](LICENSE).
