# web_knock_0
Webサービス開発のリポジトリです。

- 名前：Trampet_Laura
- グループ：C
- テーマ：テーマ0：GitとGitHubの基本・演習

- [00/](00/)
## 担当課題

| 課題番号 | 課題名 | 場所 |
|:--:|:--|:--|
| 02 | GitHubアカウントの作成，2段階認証とSSHキー登録 | [02/](02/) |

課題ごとにディレクトリ（`00/`，`01/` …）を作り，その中に成果物と説明を置いてください．

---

## 課題02：GitHubアカウントの作成，2段階認証とSSHキー登録

### やったこと

SSHキーの登録。
2段階認証はGithubのサイト上で行った。
以下のコマンドで、個人情報は***で伏せています。

### 実行結果

コマンドの出力は，スクリーンショットではなくテキストで貼り付けてください．

```
% ssh -T git@github.com
The authenticity of host 'github.com (20.27.177.113)' can't be established.
ED25519 key fingerprint is SHA256:+DiY3wvvV6TuJJhbpZisF/zLDA0zPMSvHdkr4UvCOqU.
This key is not known by any other names.
Are you sure you want to continue connecting (yes/no/[fingerprint])? いyes
Warning: Permanently added 'github.com' (ED25519) to the list of known hosts.
git@github.com: Permission denied (publickey).
% ssh-keygen -t ed25519 -C "*****@gmail.com"
Generating public/private ed25519 key pair.
Enter file in which to save the key (/Users/mapyo/.ssh/id_ed25519): 
Enter passphrase for "/Users/mapyo/.ssh/id_ed25519" (empty for no passphrase): 
Enter same passphrase again: 
Your identification has been saved in /Users/mapyo/.ssh/id_ed25519
Your public key has been saved in /Users/mapyo/.ssh/id_ed25519.pub
The key fingerprint is:
SHA256:os9vMVGTVrUG42R3/O5amIsCgeMXB76gEU8dQ15f9BY *****@gmail.com
The key's randomart image is:
+--[ED25519 256]--+
|       o+..o*o=E.|
|    . ..oo== = +o|
|     + o.+ .o o +|
|    . = = .  . ..|
|     +.oS*     . |
|    ....*      o.|
|    .  . +    o..|
|     o  . .  . o.|
|      oo.  .. o. |
+----[SHA256]-----+
% cat ~/.ssh/id_ed25519.pub
ssh-ed25519 AAAAC3NzaC1lZDI1NTE5AAAAIAx7uWnX33y9QSZncXZsuKqyrQfcGwrYicAzs3itjyzL ******@gmail.com

% ssh -T git@github.com
Hi Trumpet-Laura! You've successfully authenticated, but GitHub does not provide shell access.
```

<img width="866" height="597" alt="スクリーンショット 2026-10-23 10 32 16" src="https://github.com/user-attachments/assets/47197735-4027-4c37-968e-527a6d870523" />

### つまずいた点・調べたこと

特になし。Claudeと協働。

