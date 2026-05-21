# 🛠️ BowenAI Organization Configurations (`.github`)

This is the administrative and configuration repository for the **[BowenAI](https://github.com/BowenAI)** organization. It contains organization-wide configurations, community health files, templates, and the public organization profile.

---

## 📂 Repository Structure

* **[`profile/README.md`](file:///home/bowenson/Github/.github/profile/README.md)**: The landing page README that is displayed on the main BowenAI organization profile page.
* **[`profile/bowenai-banner.svg`](file:///home/bowenson/Github/.github/profile/bowenai-banner.svg)**: Custom brand banner assets.
* **[`.github/workflows/update-profile-readme.yml`](file:///home/bowenson/Github/.github/.github/workflows/update-profile-readme.yml)**: The automation workflow that runs daily to query all public repositories in the organization and dynamically update the profile list.

---

## ⚙️ Automated Workflows

### Update Org Profile README
* **File**: [`.github/workflows/update-profile-readme.yml`](file:///home/bowenson/Github/.github/.github/workflows/update-profile-readme.yml)
* **Schedule**: Daily at `03:00 UTC`
* **Trigger**: Can also be run manually via the **Actions** tab.
* **Function**: Uses the GitHub API to list public organization repositories, formats them, and writes them between the `<!--START-REPO-LIST-->` and `<!--END-REPO-LIST-->` placeholders in `profile/README.md`.

---

## 🤝 Contributing

To make updates to the organization profile:
1. Edit the core structure in **[`profile/README.md`](file:///home/bowenson/Github/.github/profile/README.md)** (do not manually modify the content between the `<!--START-REPO-LIST-->` tags as it will be overwritten by the bot).
2. Commit and push the changes to `main`.
3. Manually run the **Update Org Profile README** workflow in the Actions tab to update the repository list immediately.
