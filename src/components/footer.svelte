<script>
  import LogoTextless from "./svgs/logo-textless.svelte";
  const socialLinks = [
    {
      href: "https://twitter.com/gitpod",
      alt: "Twitter",
      icon: "/svg/brands/twitter.svg",
    },
    {
      href: "https://github.com/gitpod-io",
      alt: "GitHub",
      icon: "/svg/brands/github.svg",
    },
    {
      href: "https://community.gitpod.io/",
      alt: "Discourse",
      icon: "/svg/brands/discourse.svg",
    },
  ];
</script>

<div class="footer__container">
  <footer class="footer">
    <div class="footer__entries">
      <ul>
        <li>Gitpod</li>
        <li><a href="/">Home</a></li>
        <li><a href="/features">Features</a></li>
        <li><a href="/pricing">Pricing</a></li>
        <li><a href="/self-hosted">Self-Hosted</a></li>
        <li>
          <a href="/gitpod-vs-github-codespaces"
            >Gitpod vs GitHub <br />Codespaces
          </a>
        </li>
      </ul>
      <ul>
        <li>Developer</li>
        <li><a href="/#get-started">Getting started</a></li>
        <li><a href="/screencasts">Screencasts</a></li>
        <li><a href="/docs">Documentation</a></li>
        <li>
          <a
            href="https://github.com/gitpod-io/gitpod/issues/new?template=bug_report.md"
            target="_blank"
            rel="noopener">Report a bug</a
          >
        </li>
        <li>
          <a href="https://community.gitpod.io" target="_blank" rel="noopener"
            >Community
          </a>
        </li>
      </ul>
      <!-- <div style="flex: 0 0 100%">
        &nbsp;
      </div> -->
      <ul>
        <li>Company</li>
        <li><a href="/about">About</a></li>
        <li>
          <a href="/careers">Careers<sup>*</sup></a>
        </li>
        <li><a href="/contact">Contact</a></li>
      </ul>
      <ul>
        <li>Legal</li>
        <li><a href="/imprint">Imprint</a></li>
        <li>
          <a href="/terms">Terms of Service</a>
        </li>
        <li>
          <a href="/privacy">Privacy Policy</a>
        </li>
      </ul>
    </div>

    <div class="footer__bottom">
      <div class="footer__copy">
        <a href="/"
          ><div class="logo-wrapper">
            <img
              src="/svg/logo-textless.svg"
              alt="Gitpod"
              height="24"
              width="24"
            />
          </div></a
        ><span>Copyright &copy; Gitpod</span>
      </div>
      <div class="footer__social">
        {#each socialLinks as link}
          <a href={link.href} class="footer__social-link">
            <img src={link.icon} alt={link.alt} height="24" width="24" />
          </a>
        {/each}
      </div>
    </div>
  </footer>
</div>
