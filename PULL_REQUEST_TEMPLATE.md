# Pull Request

## 📋 Description

<!-- Provide a clear and concise description of your changes. -->

## 🔗 Related Issues

<!-- Link to related issues using "Fixes #123" or "Relates to #456" -->

- Fixes #
- Relates to #

## 🏷️ Type of Change

<!-- Check all that apply -->

- [ ] 🐛 **Bug Fix** — Non-breaking change that fixes an issue
- [ ] ✨ **New Feature** — Non-breaking change that adds functionality
- [ ] 💥 **Breaking Change** — Change that would cause existing functionality to not work as expected
- [ ] 📝 **Documentation** — Documentation only changes
- [ ] 🔧 **Refactor** — Code change that neither fixes a bug nor adds a feature
- [ ] 🧪 **Test** — Adding missing tests or correcting existing tests
- [ ] 🏗️ **Build/CI** — Changes to build process or CI configuration

## 📦 Affected Bindings

<!-- Check all bindings affected by this change -->

- [ ] TypeScript (Golden Master)
- [ ] Python (Release Master)
- [ ] Rust
- [ ] Go
- [ ] Java
- [ ] C/C++
- [ ] C#
- [ ] Other: <!-- specify -->
- [ ] None (documentation/tooling only)

---

## ✅ Pre-Submission Checklist

### 🏛️ Architecture Compliance

<!-- These are REQUIRED for all code changes -->

- [ ] I have read the [CONTRIBUTING.md](https://github.com/strling-lang/.github/blob/main/CONTRIBUTING.md) guide
- [ ] I have followed the **Single Source of Truth (SSOT)** workflow
- [ ] If modifying core logic: Changes were made to **TypeScript first**
- [ ] If modifying a binding: Changes pass the **Conformance Suite**

### 🧪 Testing

<!-- Check all that apply -->

- [ ] I have run `./strling test <binding>` for all affected bindings
- [ ] All new and existing tests pass locally
- [ ] I have added tests that prove my fix/feature works
- [ ] If modifying TypeScript: I have regenerated specs with `npm run build:specs`

### 📚 Documentation

- [ ] I have updated relevant documentation (README, inline comments, etc.)
- [ ] My code follows the project's style guidelines
- [ ] I have added JSDoc/docstrings for new public APIs

### 🔐 Security

- [ ] I have reviewed my changes for potential security implications
- [ ] This change does not introduce ReDoS vulnerabilities
- [ ] This change does not expose sensitive information

---

## 🔬 Omega Audit Verification

<!--
For significant changes, the Omega Audit ensures cross-binding consistency.
Fill this out if your PR modifies core compiler logic.
-->

### Test Commands Run:

```bash
# List the exact commands you ran to verify your changes
./strling test typescript
./strling test python
./strling test rust
# ...
```

### Conformance Results:

| Binding                     | Tests Passed | Tests Failed | Notes |
| :-------------------------- | :----------- | :----------- | :---- |
| TypeScript                  | ✅           | 0            |       |
| Python                      | ✅           | 0            |       |
| Rust                        | ✅           | 0            |       |
| <!-- Add more as needed --> |              |              |       |

---

## 📸 Screenshots / Examples

<!--
If applicable, add screenshots or code examples demonstrating the change.
-->

**Before:**

```strling
# Example of old behavior
```

**After:**

```strling
# Example of new behavior
```

---

## 📎 Additional Notes

<!--
Any additional context, concerns, or notes for reviewers.
- Known limitations
- Future work
- Alternative approaches considered
-->

---

## 👥 Reviewer Checklist

<!-- For maintainers reviewing this PR -->

- [ ] Code follows project architecture and style
- [ ] Changes are covered by tests
- [ ] Documentation is updated
- [ ] No security concerns
- [ ] CI/CD pipeline passes
- [ ] Ready to merge
