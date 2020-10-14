<template>
  <nav class="story-tool js-article-tool">
      <h3>Artikel-Tools</h3>
      <ul>
        <li class="js-article-tool-socialshare-menu story-tool-socialshare-menu" data-closable="story-tool-socialshare-menu" data-closable-active="false">
          <ul>
            <li class="story-tool-sharetwitter js-article-tool-share">
              <div class="story-tool-button">
                <svg viewBox="0 0 30 30"><path fill="var(--tint)" d="M12.35 24a12.24 12.24 0 0 0 12.32-12.32v-.56a8.81 8.81 0 0 0 2.15-2.24 8.65 8.65 0 0 1-2.49.68 4.35 4.35 0 0 0 1.9-2.4 8.68 8.68 0 0 1-2.75 1.05 4.33 4.33 0 0 0-7.38 3.95 12.3 12.3 0 0 1-8.92-4.52 4.33 4.33 0 0 0 1.34 5.78 4.3 4.3 0 0 1-1.97-.54v.05a4.33 4.33 0 0 0 3.48 4.25 4.32 4.32 0 0 1-1.96.07 4.34 4.34 0 0 0 4.05 3.01 8.7 8.7 0 0 1-5.38 1.86 8.82 8.82 0 0 1-1.03-.06A12.26 12.26 0 0 0 12.35 24"></path></svg>
                <span>Artikel auf Twitter teilen</span>
              </div>
            </li>
            <li class="story-tool-sharefacebook js-article-tool-share">
              <div class="story-tool-button">
                  <svg viewBox="0 0 30 30"><path fill="var(--tint)" d="M23.5 5.5h-17a1 1 0 0 0-1 1v16.9c0 .6.5 1 1 1h9.1V17h-2.5v-2.9h2.5V12c0-2.5 1.5-3.8 3.7-3.8 1 0 2 .1 2.2.1V11H20c-1.2 0-1.4.6-1.4 1.4v1.8h2.8l-.4 2.9h-2.5v7.4h4.8c.6 0 1-.5 1-1v-17c.2-.5-.3-1-.8-1z"></path></svg>
                <span>Artikel auf Facebook teilen</span>
              </div>
            </li>
            <li class="story-tool-sharewhatsapp js-article-tool-share">
              <div class="story-tool-button">
                <svg viewBox="0 0 30 30"><path fill="var(--tint)" d="M23.79 6.13A11.07 11.07 0 0 0 6.36 19.48L4.8 25.22l5.87-1.54a11.05 11.05 0 0 0 5.28 1.35 11.07 11.07 0 0 0 7.84-18.9zm-7.83 17.03a9.18 9.18 0 0 1-4.68-1.28l-.34-.2-3.48.9.93-3.38-.22-.35a9.2 9.2 0 1 1 7.79 4.3zm5.04-6.9c-.28-.13-1.64-.8-1.89-.9s-.44-.13-.62.15-.71.9-.88 1.08-.32.2-.6.07a7.56 7.56 0 0 1-2.22-1.37 8.33 8.33 0 0 1-1.53-1.92c-.17-.27-.02-.42.12-.56s.27-.32.41-.48a1.89 1.89 0 0 0 .28-.46.5.5 0 0 0-.03-.49c-.07-.14-.62-1.5-.85-2.05s-.45-.47-.62-.48h-.53a1.02 1.02 0 0 0-.74.34 3.1 3.1 0 0 0-.97 2.3 5.38 5.38 0 0 0 1.13 2.87 12.32 12.32 0 0 0 4.72 4.17 15.88 15.88 0 0 0 1.58.58 3.79 3.79 0 0 0 1.74.11 2.85 2.85 0 0 0 1.87-1.31 2.31 2.31 0 0 0 .16-1.32c-.07-.11-.25-.18-.53-.32z"></path></svg>
                <span>Artikel auf WhatsApp teilen</span>
              </div>
            </li>
          </ul>
        </li>
        <li class="story-tool-share">
          <button class="story-tool-navigatorshare js-article-tool-navigatorshare story-tool-button" title="Artikel teilen" data-share-url="https://www.derstandard.at/story/2000120860997/bluemels-budget-erntet-schon-vor-seiner-rede-kritik?ref=article" data-share-title="Wenig Investitionen, kaum Klimaschutz: Blümel erntet schon vor Rede Kritik für sein Budget" data-share-text="Der Finanzminister macht derzeit Unsummen für die Corona-Bekämpfung locker. Aus Sicht der Opposition geht die Strategie der Regierung aber nicht weit genug" hidden="">
            <svg viewBox="0 0 30 30"><path fill="var(--tint)" d="M21.3 19.3c-.8 0-1.5.3-2.1.8l-7.4-4.3c.1-.3.1-.5.1-.7 0-.3-.1-.5-.1-.8l7.4-4.3c.6.5 1.3.8 2.2.8 1.8 0 3.2-1.4 3.2-3.2s-1.4-3.2-3.2-3.2-3.2 1.4-3.2 3.2c0 .3 0 .5.1.8l-7.4 4.3c-.6-.5-1.3-.8-2.2-.8-1.8 0-3.2 1.4-3.2 3.2s1.4 3.2 3.2 3.2c.8 0 1.6-.3 2.2-.8l7.4 4.3c-.1.2-.1.4-.1.7 0 1.7 1.3 3.1 3.1 3.1s3.1-1.3 3.1-3.1-1.5-3.2-3.1-3.2z"></path></svg>
            <span>Artikel teilen</span>
          </button>
          <button class="story-tool-socialshare js-article-tool-share story-tool-button" title="Artikel teilen" data-closable-target="story-tool-socialshare-menu">
            <svg viewBox="0 0 30 30"><path fill="var(--tint)" d="M21.3 19.3c-.8 0-1.5.3-2.1.8l-7.4-4.3c.1-.3.1-.5.1-.7 0-.3-.1-.5-.1-.8l7.4-4.3c.6.5 1.3.8 2.2.8 1.8 0 3.2-1.4 3.2-3.2s-1.4-3.2-3.2-3.2-3.2 1.4-3.2 3.2c0 .3 0 .5.1.8l-7.4 4.3c-.6-.5-1.3-.8-2.2-.8-1.8 0-3.2 1.4-3.2 3.2s1.4 3.2 3.2 3.2c.8 0 1.6-.3 2.2-.8l7.4 4.3c-.1.2-.1.4-.1.7 0 1.7 1.3 3.1 3.1 3.1s3.1-1.3 3.1-3.1-1.5-3.2-3.1-3.2z"></path></svg>
            <span>Artikel teilen</span>
          </button>
        </li>
          <li class="story-tool-forum">
            <a href="#community" class="story-tool-button" data-scrollto=".story-community-postings" data-scrollto-offset="110" title="Kommentieren / Forum lesen">
              <svg viewBox="0 0 30 30"><path fill="var(--tint)" d="M4.95 9l4.9 4.9V22h14.6V9H4.95zm17.9 11.4h-11.4v-6.5c0-.4-.2-.8-.5-1.1l-2.1-2.1h14v9.7z"></path></svg>
              <span>Kommentieren / Forum lesen</span>
              <span>754 <span>Postings</span></span>
            </a>
          </li>
      </ul>
    </nav>
</template>

<script>
export default {
}
</script>

<style lang="css" scoped>
.story-tool {
  --component-name: 'editorial--story--tools';
  --background: var(--cta);
  --radius: 9px;
  --tint: var(--on-cta);
}

.story-tool h3 {
  display: none;
}

.story-tool ul {
  display: -webkit-flex;
  display: -ms-flexbox;
  display: flex;
  list-style: none;
  margin: 0;
  padding: 0;
  position: relative;
}

.story-tool li {
  box-sizing: border-box;
  display: -webkit-flex;
  display: -ms-flexbox;
  display: flex;
}

.story-tool li[hidden] {
  display: none;
}

.story-tool .story-tool-button {
  background-color: transparent;
  border-radius: 9px;
  color: #343434;
  -webkit-align-items: center;
  -ms-flex-align: center;
  align-items: center;
  background-color: var(--background);
  border: 0;
  border-radius: var(--radius);
  box-sizing: border-box;
  color: var(--tint);
  cursor: pointer;
  display: -webkit-flex;
  display: -ms-flexbox;
  display: flex;
  font-size: 1.2rem;
  -webkit-justify-content: center;
  -ms-flex-pack: center;
  justify-content: center;
  margin: 0;
  min-height: 38px;
  min-width: 38px;
  overflow: visible;
  padding: 6px;
  text-decoration: none;
}

.story-tool .story-tool-button[hidden] {
  display: none;
}

.no-touchevents .story-tool .story-tool-button:hover,
.no-touchevents .story-tool .story-tool-button:hover {
  --background: rgba(0, 0, 0, 0.1);
}

@media all and (-ms-high-contrast: none), (-ms-high-contrast: active) {
  .no-touchevents .story-tool .story-tool-button:hover,
  .no-touchevents .story-tool .story-tool-button:hover {
    background-color: #ec008c;
    color: #fff;
  }

  .no-touchevents .story-tool .story-tool-button:hover svg,
  .no-touchevents .story-tool .story-tool-button:hover svg {
    fill: #fff;
  }
}

.story-tool .story-tool-button:focus {
  outline: none;
}

.story-tool .story-tool-button > span {
  display: none;
  margin: 0 7px 0 3px;
  -webkit-transform: translateY(1px);
  transform: translateY(1px);
}

.story-tool .story-tool-button svg {
  -webkit-flex-shrink: 0;
  -ms-flex-negative: 0;
  flex-shrink: 0;
  height: 30px;
  width: 30px;
}

.story-tool .story-tool-forum .story-tool-button > span:last-of-type {
  display: inline;
  font-size: 1.5rem;
}

.story-tool .story-tool-forum .story-tool-button > span:last-of-type:empty {
  display: none;
}

.story-tool .story-tool-forum .story-tool-button > span:last-of-type span {
  display: none;
}

@media (max-width: 959.9px) {
  .story-tool {
    bottom: 15px;
    right: 15px;
    position: fixed;
    z-index: 1;
  }

  .story-tool > ul {
    background-color: #ec008c;
    border-radius: 9px;
    background-color: var(--background);
    border-radius: var(--radius);
  }
}

@media all and (max-width: 959.9px) and (-ms-high-contrast: none), (max-width: 959.9px) and (-ms-high-contrast: active) {
  .story-tool .story-tool-button {
    color: #fff;
  }

  .story-tool .story-tool-button svg {
    fill: #fff;
  }
}

@media (max-width: 959.9px) {
  .story-tool .story-tool-share {
    --radius: 0 9px 9px 0;
  }

  .story-tool .story-tool-share:last-child {
    --radius: 9px;
  }

  .story-tool .story-tool-share:last-child .story-tool-button {
    border-radius: 9px;
  }

  .story-tool .story-tool-share .story-tool-button {
    background-color: rgba(0, 0, 0, 0.3);
    border-radius: 0 9px 9px 0;
    --background: rgba(0, 0, 0, 0.3);
  }

  .no-touchevents .story-tool .story-tool-share .story-tool-button:hover,
  .no-touchevents .story-tool .story-tool-share .story-tool-button:hover {
    --background: rgba(0, 0, 0, 0.4);
  }

  .story-tool .story-tool-socialshare-menu[data-closable-active='false'] {
    display: none;
  }

  .story-tool .story-tool-socialshare-menu[data-closable-active='true'] ~ .story-tool-forum {
    display: none;
  }

  .story-tool .story-tool-socialshare-menu[data-closable-active='true'] ~ .story-tool-share:last-child {
    --radius: 0 9px 9px 0;
  }

  .story-tool .story-tool-socialshare-menu[data-closable-active='true'] ~ .story-tool-share:last-child .story-tool-button {
    border-radius: 0 9px 9px 0;
  }

  .story-tool .story-tool-socialshare-menu li {
    --radius: 0;
    margin: 0;
  }

  .story-tool .story-tool-socialshare-menu li .story-tool-button {
    border-radius: 0;
  }

  .story-tool .story-tool-socialshare-menu li:first-child {
    --radius: 9px 0 0 9px;
  }

  .story-tool .story-tool-socialshare-menu li:first-child .story-tool-button {
    border-radius: 9px 0 0 9px;
  }

  .story-tool .story-tool-sharetwitter svg,
  .story-tool .story-tool-sharefacebook svg,
  .story-tool .story-tool-sharewhatsapp svg {
    fill: #fff;
  }

  .story-tool .story-tool-sharetwitter .story-tool-button {
    background-color: #0095d2;
    --background: #0095d2;
  }

  .story-tool .story-tool-sharefacebook .story-tool-button {
    background-color: #3b5980;
    --background: #3b5980;
  }

  .story-tool .story-tool-sharewhatsapp .story-tool-button {
    background-color: #25b266;
    --background: #25b266;
  }

  .story-tool .story-tool-forum {
    --radius: 9px 0 0 9px;
    -webkit-order: -1;
    -ms-flex-order: -1;
    order: -1;
  }
}

@media (min-width: 960px) {
  .story-tool {
    --background: var(--theme-background);
    --radius: 6px;
    --tint: var(--theme-primarytint);
    opacity: 1;
    transition: opacity 100ms linear;
  }

  .collided.story-tool {
    opacity: 0;
  }

  .no-touchevents .story-tool:hover li,
  .no-touchevents .story-tool:hover li {
    width: auto;
  }

  .story-tool > ul {
    background: none;
    -webkit-flex-direction: column;
    -ms-flex-direction: column;
    flex-direction: column;
    position: -webkit-sticky;
    position: sticky;
    top: 130px;
  }
}

@media all and (min-width: 960px) and (-ms-high-contrast: none), (min-width: 960px) and (-ms-high-contrast: active) {
  .story-tool > ul {
    top: 0;
  }
}

@media (min-width: 960px) {
  .story-tool li {
    border-radius: var(--radius);
    margin: 0;
    white-space: nowrap;
    width: 42px;
  }

  .no-touchevents .story-tool li:hover,
  .no-touchevents .story-tool li:hover {
    display: block;
    width: auto;
  }

  .no-touchevents .story-tool li:hover .story-tool-button > span:first-of-type,
  .no-touchevents .story-tool li:hover .story-tool-button > span:first-of-type {
    display: inline;
    opacity: 0;
  }

  .story-tool .story-tool-share .story-tool-socialshare {
    display: none;
  }

  .no-touchevents .story-tool .story-tool-sharetwitter .story-tool-button:hover svg,
  .no-touchevents .story-tool .story-tool-sharetwitter .story-tool-button:hover svg,
  .no-touchevents .story-tool .story-tool-sharefacebook .story-tool-button:hover svg,
  .no-touchevents .story-tool .story-tool-sharefacebook .story-tool-button:hover svg,
  .no-touchevents .story-tool .story-tool-sharewhatsapp .story-tool-button:hover svg,
  .no-touchevents .story-tool .story-tool-sharewhatsapp .story-tool-button:hover svg {
    fill: #fff;
  }

  .no-touchevents .story-tool .story-tool-sharetwitter .story-tool-button:hover,
  .no-touchevents .story-tool .story-tool-sharetwitter .story-tool-button:hover {
    background-color: #0095d2;
    --background: #0095d2;
  }

  .no-touchevents .story-tool .story-tool-sharefacebook .story-tool-button:hover,
  .no-touchevents .story-tool .story-tool-sharefacebook .story-tool-button:hover {
    background-color: #3b5980;
    --background: #3b5980;
  }

  .no-touchevents .story-tool .story-tool-sharewhatsapp .story-tool-button:hover,
  .no-touchevents .story-tool .story-tool-sharewhatsapp .story-tool-button:hover {
    background-color: #25b266;
    --background: #25b266;
  }

  .story-tool .story-tool-button {
    --background: none;
    border: 2px solid transparent;
    -webkit-justify-content: flex-start;
    -ms-flex-pack: start;
    justify-content: flex-start;
    padding: 4px;
  }

  .no-touchevents .story-tool .story-tool-button:hover,
  .no-touchevents .story-tool .story-tool-button:hover {
    --background: var(--theme-primarydeco);
    --tint: var(--theme-secondarydeco);
    border-color: var(--theme-background);
  }

  .no-touchevents .story-tool .story-tool-button:hover > span:first-of-type,
  .no-touchevents .story-tool .story-tool-button:hover > span:first-of-type {
    display: inline !important;
    opacity: 1 !important;
  }

  .story-tool .story-tool-socialshare-menu > ul {
    -webkit-flex-direction: column;
    -ms-flex-direction: column;
    flex-direction: column;
  }

  .story-tool .story-tool-forum {
    -webkit-order: -1;
    -ms-flex-order: -1;
    order: -1;
    position: static;
  }

  .story-tool .story-tool-forum .story-tool-button > span:last-of-type {
    font-size: 1.8rem;
    font-weight: bold;
  }

  .story-tool .story-tool-forum .story-tool-button > span:last-of-type span {
    display: inline;
    font-size: 1.2rem;
    font-weight: normal;
  }

  .no-touchevents .story-tool .story-tool-forum .story-tool-button:hover > span:last-of-type,
  .no-touchevents .story-tool .story-tool-forum .story-tool-button:hover > span:last-of-type {
    display: none;
  }

  .no-touchevents .story-tool .story-tool-forum .story-tool-button:hover > span:first-of-type,
  .no-touchevents .story-tool .story-tool-forum .story-tool-button:hover > span:first-of-type {
    display: inline;
  }
}

.story-tool {
  -webkit-flex-grow: 1;
  -ms-flex-positive: 1;
  flex-grow: 1;
  margin: auto;
  max-width: var(--story-width);
}

@media (min-width: 960px) {
  .story-tool {
    height: 100%;
    left: -10px;
    position: absolute;
    top: -9px;
  }
}
</style>
