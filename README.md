# username.xzz.io


SET FOREIGN_KEY_CHECKS=0;

-- ----------------------------
-- Table structure for log_student_black_history
-- ----------------------------
DROP TABLE IF EXISTS `log_student_black_history`;
CREATE TABLE `log_student_black_history` (
  `id` varchar(32) NOT NULL,
  `card_no` varchar(32) NOT NULL COMMENT '卡编号',
  `card_id` varchar(32) NOT NULL DEFAULT '' COMMENT '卡序列号，刷卡时读取到的',
  `user_name` varchar(32) DEFAULT '' COMMENT '姓名',
  `create_time` datetime DEFAULT NULL COMMENT '创建时间',
  `expire_time` datetime DEFAULT NULL COMMENT '失效时间',
  PRIMARY KEY (`id`)
) ENGINE=InnoDB DEFAULT CHARSET=utf8 COMMENT='学生黑名单历史表';

-- ----------------------------
-- Records of log_student_black_history
-- ----------------------------
