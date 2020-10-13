<template>
  <div class="posting">
    <div class="posting__body">
      <h4>{{ headline }}</h4>
      <p>{{ message }}</p>
    </div>
    <div class="posting__actions">
      <div>
        <button>
          <svg style="width:24px;height:24px" viewBox="0 0 24 24">
            <path fill="currentColor" d="M19,6.41L17.59,5L12,10.59L6.41,5L5,6.41L10.59,12L5,17.59L6.41,19L12,13.41L17.59,19L19,17.59L13.41,12L19,6.41Z" />
          </svg>
        </button>
      </div>
      <div>
        <button>
          <svg style="width:24px;height:24px" viewBox="0 0 24 24">
            <path fill="currentColor" d="M14.4,6L14,4H5V21H7V14H12.6L13,16H20V6H14.4Z" />
          </svg>
        </button>
      </div>
      <div>
        <button>
          <svg style="width:24px;height:24px" viewBox="0 0 24 24">
            <path fill="currentColor" d="M12,21.35L10.55,20.03C5.4,15.36 2,12.27 2,8.5C2,5.41 4.42,3 7.5,3C9.24,3 10.91,3.81 12,5.08C13.09,3.81 14.76,3 16.5,3C19.58,3 22,5.41 22,8.5C22,12.27 18.6,15.36 13.45,20.03L12,21.35Z" />
          </svg>
        </button>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  props: ['headline', 'message']
}
</script>

<style lang="scss">
.posting {
  background: var(--posting-background);
  border: 1px solid var(--border-color);
  margin-bottom: 15px;

  .posting__body {
    padding: 15px;

    h4, p {
      margin: 0 0 6px;
    }
  }

  .posting__actions {
    border-top: 1px solid var(--border-color);
    display: flex;

    div {
      flex-grow: 1;

      &:nth-child(2) {
        border-width: 0 1px;
        border-color: var(--border-color);
        border-style: solid;
      }
    }

    button {
      border: 0;
      background: 0;
      height: 35px;
      line-height: 0;
      width: 100%;
    }
  }
}
</style>
