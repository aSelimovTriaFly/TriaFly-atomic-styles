<script>
    import { Highlight } from "svelte-highlight"
    import { xml } from "svelte-highlight/languages"
</script>

<div id="align-table" class="mb-4">
    <div class="h4" role="heading" aria-level="4">Table sell wrap</div>
    <div class="d-inline-block rounded-2 bg-error mb-4 p-4">
        <i class="fas fa-exclamation-circle"></i> Please note that <b>.align-baseline</b>, <b>.align-text-top</b> and <b>.align-text-bottom</b> do not affect the behavior of the container.
    </div>
    <div class="rounded-2 overflow-hidden">
        <div class="bg-positive rounded-2 rounded-bottom-0 p-4 text-center">
            <table class="mx-auto" style="height: 120px;">
                <tr>
                    <td class="bg-error p-4 align-baseline">baseline</td>
                    <td class="p-4 align-top">top</td>
                    <td class="p-4 align-middle">middle</td>
                    <td class="p-4 align-bottom">bottom</td>
                    <td class="bg-error p-4 align-text-top">text-top</td>
                    <td class="bg-error p-4 align-text-bottom">text-bottom</td>
                </tr>
            </table>
        </div>
        <Highlight
            class="my-0"
            language='{xml}'
            code='
    <table>
        <tr>
            <td class="align-baseline">.align-baseline</td>
            <td class="align-top">.align-top</td>
            <td class="align-middle">.align-middle</td>
            <td class="align-bottom">.align-bottom</td>
            <td class="align-text-top">.align-text-top</td>
            <td class="align-text-bottom">.align-text-bottom</td>
        </tr>
    </table>
            '
        />
    </div>
</div>
