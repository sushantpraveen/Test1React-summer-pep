import React, { useState } from "react";

const Tabs = ({ tabs }) => {
  const [activeTab, setActiveTab] = useState(0);

  const handleClick = (index) => {
    setActiveTab(index);
  };

  return (
    <div>
      <ul>
        {tabs.map((tab, index) => (
          <li key={index} onClick={() => handleClick(index)}>
            {tab.title}
          </li>
        ))}
      </ul>
      <div>{tabs[activeTab].content}</div>
    </div>
  );
};

const App = () => {
  const tabs = [
    { title: "Tab 1", content: "This is the content for Tab 1" },
    { title: "Tab 2", content: "Tab 2" },
    { title: "Tab 3", content: "Tab 3" },
  ];

  return <Tabs tabs={tabs} />;
};

export default App;
