The version system you're referring to is commonly known as **Semantic Versioning**, or **SemVer** for short. It helps developers understand how changes to software might affect compatibility.

A version number like `1.0.0` typically follows the format:

`MAJOR.MINOR.PATCH`

Each of these segments has a specific meaning:

---

### 1. MAJOR version (e.g., `1.x.x`)

- Changes that break backward compatibility.
- When incremented, it signals that old code relying on the previous version may no longer work.
    
- Example:
    - Changing how a public function works.
    - Removing features or APIs.

**Going from `1.4.2` → `2.0.0` means:** a major change occurred, and developers need to adapt their code to use this new version.

---

### 2. MINOR version (e.g., `x.1.x`)

- New features added in a backward-compatible manner.
- No breaking changes — existing functionality continues to work as before.
    
- Example:
    - Adding a new function.
    - Improving performance.
    - Expanding an API.

**Going from `1.4.2` → `1.5.0` means:** new functionality is available, but nothing should break.

---

### 3. PATCH version (e.g., `x.x.2`)

- **Bug fixes or small backward-compatible improvements.**
    
- No new features, just maintenance.
    
- Example:
    
    - Fixing a typo or logic bug.
        
    - Improving documentation or performance without changing functionality.
        

**Going from `1.4.2` → `1.4.3` means:** a fix or tweak was made, no features added.

---

### Bonus: Pre-release & Build Metadata

Semantic versioning can also include extra info:

- **Pre-release identifiers** (`-alpha`, `-beta`, `-rc.1`, etc.)
    
    - `1.0.0-alpha` is less stable than `1.0.0-beta`, which is less stable than `1.0.0-rc.1` (release candidate).
        
- **Build metadata** (`+build.456`)
    
    - Non-functional, used for internal tracking.
        

Example:

matlab

CopyEdit

`1.2.0-beta.3+exp.sha.5114f85`