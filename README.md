# Deploy with Surge.sh

A simple Github Actions template to deploy your static site using [Surge.sh](https://surge.sh).

## Steps

**1**. Obtain a development token from [Surge.sh](https://surge.sh).

```bash
npx surge token
```

**2**. Setup _secrets_ within your repository.

- **SURGE_LOGIN**: _Username_ / _email address_ attached to your [Surge.sh](https://surge.sh) account.

-	**SURGE_TOKEN**: The development token obtained from _Step 1_.

-	**SURGE_DOMAIN**: The domain you want to publish your site too.
	- _For example_: `<domain-name-here>.surge.sh` or `<domain-name-here>.com`

**3**. Add [`deployment.yml`](deployment.yml) to the `.github/workflows` directory contained at the root of your project.

**4**. Test the workflow with a commit to the _master_ branch.

## License

© 2020 Nicholas Adamou.

It is free software, and may be redistributed under the terms specified in the [LICENSE] file.

[license]: LICENSE
