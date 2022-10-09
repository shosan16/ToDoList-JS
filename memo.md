  const clickAddTask = () => {
    document.getElementById("add-button").addEventListener("click", () => {
      const text = document.getElementById("add-text").value;
      console.log(text);

      const div = document.createElement("div");
      div.className = "list-row";
      const li = document.createElement("li");
      li.innerHTML = text;

      div.appendChild(li);

      const ul = document.getElementById("incomplete-list");
      ul.appendChild(div);
    });
  };
  clickAddTask();



## 完了削除ボタン
  const completeButton = document.createElement("button");
  completeButton.innerHTML = "完了";
  completeButton.addEventListener("click", () => {
    div.parentNode.removeChild(div);
    document.getElementById("complete-list").appendChild(div);
  });

  const deleteButton = document.createElement("button");
  deleteButton.innerHTML = "削除";
  deleteButton.addEventListener("click", () => {
    div.parentNode.removeChild(div);
  });