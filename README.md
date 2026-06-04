<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0a0a0a,50:0a0a0a,100:2DD4BF&height=240&section=header&text=ZKSend&fontSize=88&fontColor=ffffff&fontAlignY=38&desc=stealth%20addresses%20on%20solana&descAlignY=62&descSize=18&animation=fadeIn" width="100%" alt="banner"/>

<a href="https://github.com/ZKSend-proto">
<img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=600&size=20&pause=1000&color=2DD4BF&center=true&vCenter=true&width=720&lines=ECDH+on+ed25519;view-key+recoverable;no+relayer+%C2%B7+no+mixer+%C2%B7+no+custom+contract;solana+memo+program+is+the+only+footprint" alt="typing"/>
</a>

<br/><br/>

<a href="https://github.com/ZKSend-proto"><img src="https://komarev.com/ghpvc/?username=ZKSend-proto&label=profile+views&color=2DD4BF&style=flat-square" alt="views"/></a>
<a href="https://x.com/ZKSend"><img src="https://img.shields.io/badge/twitter-@ZKSend-2DD4BF?style=flat-square&logo=x&logoColor=ffffff&labelColor=0a0a0a" alt="twitter"/></a>
<a href="https://zksend.xyz"><img src="https://img.shields.io/badge/site-zksend.xyz-2DD4BF?style=flat-square&labelColor=0a0a0a" alt="site"/></a>

</div>

<br/>

<div align="center">
<picture>
<source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/ZKSend-proto/ZKSend-proto/output/github-contribution-grid-snake-dark.svg">
<img alt="snake" src="https://raw.githubusercontent.com/ZKSend-proto/ZKSend-proto/output/github-contribution-grid-snake.svg" width="100%"/>
</picture>
</div>

<br/>

## ⌬ &nbsp; what

ZKSend is a stealth-address protocol on Solana. Each payment lands on a fresh
one-time address derived in the payer's browser via ECDH on ed25519. Only the
recipient view-key can detect and claim them. No relayer, no mixer, no custom
on-chain program — the only footprint is a 48-character memo.

```
1. recipient generates an ed25519 meta-keypair in browser
2. meta-pub is published as a URL fragment (zksend.xyz/pay#m=...)
3. sender opens the link, derives a one-time stealth address via ECDH
4. sender transfers SOL to stealth_addr + memo "nt1:<eph_pub>"
5. recipient scans memos, applies ECDH with their meta-priv
6. on match: derives the spend scalar, sweeps to main wallet
```

<br/>

## ⌬ &nbsp; stack

<div align="center">
<img height="170" src="https://github-readme-stats.vercel.app/api?username=ZKSend-proto&show_icons=true&theme=transparent&hide_border=true&bg_color=0a0a0a&title_color=2DD4BF&icon_color=2DD4BF&text_color=f2f2f2&include_all_commits=true&rank_icon=github"/>
<img height="170" src="https://github-readme-stats.vercel.app/api/top-langs/?username=ZKSend-proto&layout=compact&theme=transparent&hide_border=true&bg_color=0a0a0a&title_color=2DD4BF&text_color=f2f2f2&langs_count=6"/>
</div>

<br/>

## ⌬ &nbsp; pinned

<table>
<tr>
<td width="50%" valign="top">

<a href="https://github.com/ZKSend-proto/stealth-sdk"><img src="https://github-readme-stats.vercel.app/api/pin/?username=ZKSend-proto&repo=stealth-sdk&theme=transparent&hide_border=true&title_color=2DD4BF&icon_color=2DD4BF&text_color=f2f2f2&bg_color=0a0a0a"/></a>

</td>
<td width="50%" valign="top">

<a href="https://github.com/ZKSend-proto/stealth-core"><img src="https://github-readme-stats.vercel.app/api/pin/?username=ZKSend-proto&repo=stealth-core&theme=transparent&hide_border=true&title_color=2DD4BF&icon_color=2DD4BF&text_color=f2f2f2&bg_color=0a0a0a"/></a>

</td>
</tr>
<tr>
<td width="50%" valign="top">

<a href="https://github.com/ZKSend-proto/zksend-wallet"><img src="https://github-readme-stats.vercel.app/api/pin/?username=ZKSend-proto&repo=zksend-wallet&theme=transparent&hide_border=true&title_color=2DD4BF&icon_color=2DD4BF&text_color=f2f2f2&bg_color=0a0a0a"/></a>

</td>
<td width="50%" valign="top">

<a href="https://github.com/ZKSend-proto/stealth-scanner"><img src="https://github-readme-stats.vercel.app/api/pin/?username=ZKSend-proto&repo=stealth-scanner&theme=transparent&hide_border=true&title_color=2DD4BF&icon_color=2DD4BF&text_color=f2f2f2&bg_color=0a0a0a"/></a>

</td>
</tr>
</table>

<br/>

## ⌬ &nbsp; references

- ERC-5564 — Stealth Address Standard
- Solana Memo Program — `MemoSq4gqABAXKb96qnH8TysNcWxMyWCqXgDLGmfcHr`
- `@noble/curves` — audited curve crypto

<br/>

<div align="center">
<img src="https://capsule-render.vercel.app/api?type=waving&color=0:2DD4BF,50:0a0a0a,100:0a0a0a&height=120&section=footer&animation=fadeIn" width="100%" alt="footer"/>
</div>

<!-- docs: link pinned repos in tagline area -->
<!-- docs: add 'what' section explaining protocol -->
<!-- docs: tweak banner gradient stops -->