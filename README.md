# macOS Geliştirici Araçları Kurulum Playbook'u

Bu Ansible playbook'u, macOS'ta geliştirme ortamınızı hızlıca kurmanızı sağlar. Aşağıdaki araçları otomatik olarak kurar:

- VS Code
- Slack
- GitHub Desktop
- Postman
- Google Chrome
- AnyDesk
- FortiClient VPN
- Microsoft Outlook
- Node.js (nvm ile)

## Proje Yapısı

```
mac-dev-bootstrapper/
├── README.md
├── inventory/
│   └── localhost
└── playbook.yml
```

## Özellikler

- Homebrew otomatik kurulumu
- GUI uygulamalarının otomatik kurulumu
- Node.js kurulumu (nvm ile)
- Gerekli Ansible koleksiyonlarının otomatik kurulumu

## Gereksinimler

- macOS işletim sistemi
- Ansible

## Kurulum

1. Ansible'ı yükleyin:
```bash
brew install ansible
```

2. Projeyi klonlayın:
```bash
git clone https://github.com/sakiphan/mac-dev-bootstrapper.git
cd mac-dev-bootstrapper
```

3. Playbook'u çalıştırın:
```bash
ansible-playbook -i inventory/localhost playbook.yml
```

## Notlar

- Playbook çalıştığında Homebrew otomatik olarak kurulacaktır
- Node.js, nvm (Node Version Manager) üzerinden kurulacaktır
- Kurulumlar tamamlandıktan sonra terminali yeniden başlatmanız gerekebilir 