# Refex PWA - Offline Trip Management

Complete offline-first Progressive Web App (PWA) for ERPNext Trip doctype management.

## 🚀 Repository

**GitHub**: [https://github.com/raghulje/refex_pwa.git](https://github.com/raghulje/refex_pwa.git)

## 📋 Quick Start

```bash
# Clone the repository
git clone https://github.com/raghulje/refex_pwa.git
cd refex_pwa

# Install in ERPNext bench
bench get-app refex_pwa https://github.com/raghulje/refex_pwa.git
bench install-app refex_pwa

# Build assets
bench build --app refex_pwa
bench restart
```

## ✨ Features

- ✅ **100% Offline Support** - Work without internet
- ✅ **Auto-Save** - Saves every 5 seconds when offline
- ✅ **Auto-Sync** - Syncs when connection restored
- ✅ **File Uploads** - Upload files offline
- ✅ **Complete Trip Management** - Create/edit/delete trips offline
- ✅ **All Reference Data Cached** - Projects, Items, Suppliers, etc.
- ✅ **Mobile Installable** - Install as native app
- ✅ **100+ Features** - Production-ready

## 📁 Project Structure

```
refex_pwa/
├── public/
│   ├── manifest.json          # PWA manifest
│   ├── sw.js                  # Service Worker
│   └── js/
│       ├── pwa-init.js        # PWA initialization
│       ├── offline-db.js      # IndexedDB wrapper
│       ├── offline-sync.js    # Sync manager
│       ├── offline-files.js   # File upload handler
│       ├── offline-listview.js # List view support
│       └── trip-offline.js    # Trip form handler
├── refex/
│   └── api.py                 # Backend sync APIs
├── hooks.py                   # ERPNext hooks
└── Documentation/
    ├── SETUP_OFFLINE_PWA.md
    ├── PWA_FEATURES_LIST.md
    ├── OFFLINE_COMPLETE_FEATURES.md
    └── OFFLINE_PWA_SOLUTION.md
```

## 📚 Documentation

- **[Setup Guide](SETUP_OFFLINE_PWA.md)** - Quick setup instructions
- **[Features List](PWA_FEATURES_LIST.md)** - Complete features list
- **[Offline Features](OFFLINE_COMPLETE_FEATURES.md)** - What works offline
- **[Solution Overview](OFFLINE_PWA_SOLUTION.md)** - Complete solution details

## 🎯 Use Case

Perfect for:
- Rural areas with poor internet connectivity
- Field workers entering trip data
- Sites with unreliable connections
- Mobile-first workflows

## 🔧 Development

### Adding New Features

1. Make changes in local repository
2. Test thoroughly
3. Commit changes
4. Push to repository:
   ```bash
   git push pwa develop:main
   ```

### Remote Setup

```bash
# Add remote (already configured)
git remote add pwa https://github.com/raghulje/refex_pwa.git

# Push to PWA repository
git push pwa develop:main
```

## 📝 License

MIT License

## 👥 Contributors

- Initial PWA implementation for Refex ERPNext app

## 🔗 Links

- **Repository**: https://github.com/raghulje/refex_pwa.git
- **ERPNext**: https://frappeframework.com/
- **PWA Documentation**: https://web.dev/progressive-web-apps/

---

**Ready for production use in rural areas with poor connectivity!** 🎉

