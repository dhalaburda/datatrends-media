# Public media setup

This repository is public. Every committed file, including files outside public/, is publicly accessible through GitHub. Never add tokens, private drafts, sensitive screenshots or client-confidential material. Deletion does not remove Git history or third-party copies.

## Enable Pages

In repository Settings > Pages > Build and deployment, select GitHub Actions as the source. Then open Actions > Deploy public media > Run workflow on main. If the initial push run fails before Pages is enabled, run it again after selecting the source.

The workflow publishes only public/. It does not access the Threads token, modify another repository or publish Threads posts.

## Add an approved image

Use Add file > Upload files to put an approved JPG or PNG in public/threads/. For example, public/threads/intro-001-v1.jpg. Commit to main and wait for Deploy public media to succeed.

With the default project Pages address and no custom domain, the example image URL will be:
https://dhalaburda.github.io/datatrends-media/threads/intro-001-v1.jpg

That image is not included in this setup. The URL will not work until the image has been uploaded and deployment succeeds. Open the deployed image URL without signing in before adding it to a private draft. Threads compatibility must be tested separately.

Use a new versioned filename when changing an image. Review for personal information, confidential data, embedded metadata and rights to publish before committing. Only approved public assets belong here. Do not put instructions or private notes inside public/.

The private datatrends-threads repository remains responsible for draft review and future publishing. This setup does not enable live Threads publishing.
