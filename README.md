# Board Games Online Hub

Trang web tổng hợp (Game Portal) dẫn tới 5 tựa Board Game & Party Game trực tuyến của **Nguyên Khang (KennyPhan)**:

| Game | Số người chơi | Link chơi trực tiếp | GitHub Repo |
|------|--------------|---------------------|-------------|
| **Coup** | 2–6 người | [coup-online.pnk.workers.dev](https://coup-online.pnk.workers.dev/) | [KennyPhan123/coup-online](https://github.com/KennyPhan123/coup-online) |
| **Decrypto** | 3–8+ người | [decrypto.pnk.workers.dev](https://decrypto.pnk.workers.dev/) | [KennyPhan123/decrypto-online](https://github.com/KennyPhan123/decrypto-online) |
| **Skull** | 3–6 người | [skull-online.pnk.workers.dev](https://skull-online.pnk.workers.dev/) | [KennyPhan123/skull-online](https://github.com/KennyPhan123/skull-online) |
| **Spicy** | 2–6 người | [spicy-online.pnk.workers.dev](https://spicy-online.pnk.workers.dev/) | [KennyPhan123/spicy-online](https://github.com/KennyPhan123/spicy-online) |
| **That's Not a Hat!** | 2–8 người | [thats-not-a-hat-online.pnk.workers.dev](https://thats-not-a-hat-online.pnk.workers.dev/) | [KennyPhan123/thats-not-a-hat-online](https://github.com/KennyPhan123/thats-not-a-hat-online) |

## Cách triển khai (Deploy)

### Cách 1: Cloudflare Workers (cùng tên miền `.pnk.workers.dev` với 5 game)
```bash
cd board-games-hub
npx wrangler login
npx wrangler deploy
```
Sau khi chạy xong, bạn sẽ có một link duy nhất: **`https://board-games.pnk.workers.dev/`**

### Cách 2: GitHub Pages
1. Tạo repo mới trên GitHub (ví dụ `board-games` hoặc `board-games-hub`).
2. Push thư mục này lên GitHub:
   ```bash
   git remote add origin https://github.com/KennyPhan123/board-games-hub.git
   git push -u origin main
   ```
3. Vào **Settings → Pages** của repo, chọn nhánh `main` (`/root`) để lấy link `https://kennyphan123.github.io/board-games-hub/`.
