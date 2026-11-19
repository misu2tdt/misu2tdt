# Hi, I'm Tien 👋

Final-year Computer Science student at HCMUT. I build backend systems and care about the parts that break under real use: concurrent writes, retried requests, and rate limits.

**Looking for:** a Backend Developer internship in Ho Chi Minh City.

---

## Featured projects

### [VERVE Studio](https://github.com/misu2tdt/ecommerce-backend): e-commerce platform
*The problem:* two customers buying the last item at once, and payment callbacks that arrive twice or after an order has expired.

- Checkout uses PostgreSQL row-level locks on stock, payment and order rows. I reproduced a payment **deadlock** in a test and fixed it by changing the lock order.
- Payments are safe to retry through **idempotency keys** and a rule of one active payment per order. Late callbacks go to an admin reconciliation list.
- 700+ backend tests plus Playwright smoke tests run in GitHub Actions.

`NestJS` `PostgreSQL` `Next.js` `JWT` · [Backend](https://github.com/misu2tdt/ecommerce-backend) · [Frontend](https://github.com/misu2tdt/ecommerce-frontend) · [Live demo](https://ecommerce-frontend-kappa-sage.vercel.app)

### [ExtProbe](https://github.com/misu2tdt/ExtProbe): Chrome extension behavior sandbox
*The question:* which requests does a Chrome extension really send, where, and with what data?

- A Python CLI runs the extension in a disposable Docker container and exports an HTML/JSON report with evidence.
- Requests are attributed to service workers, content scripts or pages using Chrome DevTools Protocol initiators. Scoring runs offline, so saved traces can be re-scored.
- Analyzed about 900 real extensions; 121 automated tests run in CI.

`Python` `Docker` `Playwright` `CDP` · [Code](https://github.com/misu2tdt/ExtProbe) · [Demo video](https://youtu.be/vBHNPCh5fcg)

---

## Stack

**Languages:** TypeScript, JavaScript, Python, SQL
**Backend:** NestJS, Node.js, REST, JWT, TypeORM, Swagger/OpenAPI
**Data:** PostgreSQL, Redis
**Tooling:** Docker, GitHub Actions, Jest, Playwright, Git

## GitHub stats

<p align="left">
  <img src="https://github-readme-stats.vercel.app/api?username=misu2tdt&show_icons=true&theme=radium&hide_border=true" alt="GitHub stats" />
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=misu2tdt&layout=compact&theme=radium&hide_border=true" alt="Top languages" />
</p>

## Education

HCMUT, VNU-HCM · B.Sc. Computer Science · Oct 2022 – Nov 2027 (expected) · TOEIC 730

## Contact

[tdtien7a1@gmail.com](mailto:tdtien7a1@gmail.com) · [LinkedIn](https://www.linkedin.com/in/tien-tran-256169242/)
