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

With the three metrics repositories checked out as siblings, validate the complete
publication input with:

```console
dotnet run --project ../sdeveng-metrics-tooling/src/SdevEng.Metrics -- \
  publish-pages ../sdeveng-metrics-dashboard public _site
```

## License

MIT. See [LICENSE](LICENSE).
