<script setup lang="ts">
import dayjs from 'dayjs'

const currentYear = ref(dayjs().year())

const { t } = useI18n()
</script>

<template>
  <ALayoutFooter class="bg-[--color-bg-2] px-2">
    <div
      class="mx-auto flex h-14 w-256 max-w-full whitespace-nowrap flex items-center justify-center"
    >
      <ASpace>
        <div>
          Copyright &copy; {{ currentYear }}
          <ALink target="_blank" href="https://wjx.im">
            老汪博客
          </ALink>
        </div>
        <div>
          Code with by
          <ALink target="_blank" href="https://www.ikxin.com">
            {{ t('label.author') }}
          </ALink>
        </div>
      </ASpace>
    </div>
  </ALayoutFooter>
</template>
