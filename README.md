
# 🗂️ FileTreeSim: A Python-Based Hierarchical File System Emulator

**FileTreeSim** is a Python module that emulates a hierarchical file system using a tree-based structure. It allows the creation and manipulation of drives, directories, and files, supporting common operations like navigating paths, copying, cutting, deleting, and renaming nodes—all within an in-memory structure.

### 🚀 Features

- 🧱 **Tree-based architecture** with `DirNode` and `FileNode` classes
- 🖥️ Simulates a file system rooted at `"This PC"` with configurable storage size
- 📁 Create and manage drives and folders (`mkdir`, `mkdrive`)
- 📄 Add and manage files (`mkfile`)
- 📂 Copy-paste and cut-paste operations with conflict resolution
- 🧭 Navigation support (`cd`, forward/backward, reset to root)
- 🗑️ Recursive delete
- 💾 Save/load session using `pickle`
- 🌲 Visualize the structure using the `pptree` library

### 📦 Usage Example

```python
fs = FileSystem(100)
fs.mkdrive("C", 30)
fs.cd_name("C")
fs.mkdir("Documents")
fs.mkfile("notes", "txt")
fs.show()
```

### 📚 Dependencies

- `pptree` – For pretty-printing the tree structure
- Python ≥ 3.6

---

Let me know if you want a shorter version or a `README.md` with usage instructions and examples!
