<script>
    import { Highlight } from "svelte-highlight"
    import { xml } from "svelte-highlight/languages"
</script>

<div id="warning" class="mb-4">
    <div class="h3" role="heading" aria-level="3">Warning</div>
    <div class="rounded-2 overflow-hidden">
        <div class="bg-positive rounded-2 rounded-bottom-0 p-4 text-center">
            <div class="d-inline-flex g-4 flex-wrap">
                <button class="tf_btn tf_btn-warning">warning button</button>
                <button class="tf_btn tf_btn-warning"><i class="fas fa-home"></i> icon button</button>
                <button class="tf_btn tf_btn-warning active">active button</button>
                <button class="tf_btn tf_btn-warning" disabled>disabled button</button>
            </div>
        </div>
        <Highlight class="my-0"
            language='{xml}'
            code='
    // warning color button
    <button class="tf_btn tf_btn-warning">info button</button>
    
    // warning color button with icon
    <button class="tf_btn tf_btn-warning">
        <i class="fas fa-home"></i>
        icon button
    </button>

    // active button
    <button class="tf_btn tf_btn-warning active">active button</button>

    // warning color disabled button
    <button class="tf_btn tf_btn-warning" disabled>disabled button</button>
            '
        />
    </div>
</div>