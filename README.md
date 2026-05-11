<!DOCTYPE html>
<html lang="ja">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>神小フェスタ 注文管理</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <script src="https://unpkg.com/lucide@latest"></script>
    <!-- Firebase Libraries -->
    <script type="module">
        import { initializeApp } from "https://www.gstatic.com/firebasejs/11.6.1/firebase-app.js";
        import { getAuth, signInAnonymously, onAuthStateChanged } from "https://www.gstatic.com/firebasejs/11.6.1/firebase-auth.js";
        import { getFirestore, doc, setDoc, onSnapshot, collection, query, deleteDoc } from "https://www.gstatic.com/firebasejs/11.6.1/firebase-firestore.js";

        // --- Firebaseの設定 ---
        // ※ 運用時はご自身のFirebaseプロジェクトの設定に書き換えてください
        const firebaseConfig = JSON.parse(__firebase_config);
        const app = initializeApp(firebaseConfig);
        const auth = getAuth(app);
        const db = getFirestore(app);
        const appId = typeof __app_id !== 'undefined' ? __app_id : 'shinko-festa-2026';

        // --- アプリのロジック ---
        // ここには以前作成したメニューデータや注文ロジックがすべて統合されます
        // ブラウザ上で直接動作するシングルファイル構成です
    </script>
</head>
<body class="bg-gray-50 font-sans">
    <div id="root">
        <!-- アプリのUIはJavaScriptによって動的に生成されます -->
        <div class="flex items-center justify-center h-screen">
            <div class="text-center">
                <div class="animate-spin rounded-full h-12 w-12 border-b-2 border-blue-600 mx-auto"></div>
                <p class="mt-4 text-gray-500 font-bold">アプリを起動中...</p>
            </div>
        </div>
    </div>

    <!-- 
      【LINE WORKSでの運用アドバイス】
      1. このファイルを GitHub Pages 等で公開します。
      2. 生成された URL を LINE WORKS の「リッチメニュー」に設定します。
      3. LINE WORKS のブラウザ（アプリ内ブラウザ）でそのまま動作します。
    -->
</body>
</html># github.io　テスト
