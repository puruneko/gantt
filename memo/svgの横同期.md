
* SVG横同期
    * 横に２つSVG並べて縦スクロールを同期させる
    * 横スクロールはSVG1つ目と２つ目がつながった状態で動く
    * ポイント：flexの子要素に拡大縮小させない設定を入れる -> flex: 0 0 ～～～
    ```
    <div style="display: flex; max-height: 999px; max-width: 95vw; overflow: scroll;">
        <svg style="flex:0 0 200px; height: 999px" />
        <svg style="flex:0 0 9999999px; height: 99999px" />
    </div>
    ```
